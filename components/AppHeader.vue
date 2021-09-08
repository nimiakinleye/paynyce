<template>
  <div class="">
    <div
      :class="{ bgBlur: positionMd }"
      class="hidden fixed top-0 z-40 px-4 lg:px-16 py-3 md:flex items-center justify-between w-full"
    >
      <nuxt-link to="/">
        <img class="w-12" src="~/assets/logo.svg" alt="">
      </nuxt-link>
      <div class="text-black links">
        <nuxt-link to="/" class="pb-1 hover:bg-white hover:text-gray-800 px-3 py-1">Home</nuxt-link>
        <nuxt-link class="ml-3 lg:ml-12 pb-1 hover:bg-white hover:text-gray-800 px-3 py-1" to="#about">About</nuxt-link>
        <nuxt-link class="ml-3 lg:ml-12 pb-1 hover:bg-white hover:text-gray-800 px-3 py-1" to="#subsidiaries">Subsidiaries</nuxt-link>
        <nuxt-link class="ml-3 lg:ml-12 my-bg px-6 py-2 rounded text-white" to="#contact-us"
          >Lets Talk</nuxt-link
        >
      </div>
    </div>
    <div class="fixed top-0 w-full z-40 md:hidden block">
      <div
        :class="{ bgBlur: positionMd }"
        class="items-center flex justify-between px-2 py-3"
      >
        <nuxt-link class="w-8" to="/">
          <img class="w-12" src="~/assets/logo.svg" alt="">
        </nuxt-link>
        <div @click="toggleNav" class="cursor-pointer" v-html="navSvg">
          
        </div>
      </div>
      <div
        id="nav"
        :class="{ showNav: showNav, hideNav: !showNav }"
        class="flex flex-col divide-y-2 rounded-b-lg divide-black items-center bg-white bg-opacity-70 py-3"
      >
        <div @click="toggleNav" class="py-2">
          <nuxt-link to="/">Home</nuxt-link>
        </div>
        <div @click="toggleNav" class="py-2">
          <nuxt-link to="#about">About</nuxt-link>
        </div>
        <div @click="toggleNav" class="py-2">
          <nuxt-link to="#subsidiaries">Subsidiaries</nuxt-link>
        </div>
        <div @click="toggleNav" class="py-2">
          <nuxt-link to="#contact-us">Let's Talk</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
  },
  data() {
    return {
      position: true,
      positionMd: false,
      showNav: false,
      navSvg: `<svg
            class="w-8 fill-current my-color"
            viewBox="0 0 512 512"
            style="enable-background: new 0 0 512 512"
            xml:space="preserve"
          >
            <g transform="translate(1 1)">
              <g>
                <g>
                  <path
                    d="M255-1C113.618-1-1,113.618-1,255s114.618,256,256,256s256-114.618,256-256S396.382-1,255-1z M255,468.333     c-117.818,0-213.333-95.515-213.333-213.333S137.182,41.667,255,41.667S468.333,137.182,468.333,255S372.818,468.333,255,468.333     z"
                  />
                  <path
                    d="M361.667,148.333H148.333c-11.782,0-21.333,9.551-21.333,21.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,157.885,373.449,148.333,361.667,148.333z"
                  />
                  <path
                    d="M361.667,233.667H148.333C136.551,233.667,127,243.218,127,255s9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333S373.449,233.667,361.667,233.667z"
                  />
                  <path
                    d="M361.667,319H148.333C136.551,319,127,328.551,127,340.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,328.551,373.449,319,361.667,319z"
                  />
                </g>
              </g>
            </g>
          </svg>`,
    }
  },
  methods: {
    onScroll() {
      if (window.pageYOffset > 250) {
        this.position = true
        this.positionMd = true
      } else {
        this.position = false
        this.positionMd = false
      }
    },
    toggleNav() {
      if (this.showNav === false) {
        this.showNav = true;
        this.navSvg = `<svg
            class="w-8 fill-current my-color"
            viewBox="0 0 340.8 340.8"
            style="enable-background: new 0 0 340.8 340.8"
            xml:space="preserve"
          >
            <g>
              <g>
                <path
                  d="M170.4,0C76.4,0,0,76.4,0,170.4s76.4,170.4,170.4,170.4s170.4-76.4,170.4-170.4S264.4,0,170.4,0z M170.4,323.6    c-84.4,0-153.2-68.8-153.2-153.2S86,17.2,170.4,17.2S323.6,86,323.6,170.4S254.8,323.6,170.4,323.6z"
                />
              </g>
            </g>
            <g>
              <g>
                <path
                  d="M182.4,169.6l50-50c3.2-3.2,3.2-8.8,0-12c-3.2-3.2-8.8-3.2-12,0l-50,50l-50-50c-3.2-3.2-8.8-3.2-12,0    c-3.2,3.2-3.2,8.8,0,12l50,50l-50,49.6c-3.2,3.2-3.2,8.8,0,12c1.6,1.6,4,2.4,6,2.4s4.4-0.8,6-2.4l50-50l50,50c1.6,1.6,4,2.4,6,2.4    s4.4-0.8,6-2.4c3.2-3.2,3.2-8.8,0-12L182.4,169.6z"
                />
              </g>
            </g>
          </svg>`
      } else {
        this.showNav = false;
        this.navSvg = `<svg
            class="w-8 fill-current my-color"
            viewBox="0 0 512 512"
            style="enable-background: new 0 0 512 512"
            xml:space="preserve"
          >
            <g transform="translate(1 1)">
              <g>
                <g>
                  <path
                    d="M255-1C113.618-1-1,113.618-1,255s114.618,256,256,256s256-114.618,256-256S396.382-1,255-1z M255,468.333     c-117.818,0-213.333-95.515-213.333-213.333S137.182,41.667,255,41.667S468.333,137.182,468.333,255S372.818,468.333,255,468.333     z"
                  />
                  <path
                    d="M361.667,148.333H148.333c-11.782,0-21.333,9.551-21.333,21.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,157.885,373.449,148.333,361.667,148.333z"
                  />
                  <path
                    d="M361.667,233.667H148.333C136.551,233.667,127,243.218,127,255s9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333S373.449,233.667,361.667,233.667z"
                  />
                  <path
                    d="M361.667,319H148.333C136.551,319,127,328.551,127,340.333c0,11.782,9.551,21.333,21.333,21.333h213.333     c11.782,0,21.333-9.551,21.333-21.333C383,328.551,373.449,319,361.667,319z"
                  />
                </g>
              </g>
            </g>
          </svg>`
      }
    },
  },
  beforeMount() {
    window.addEventListener('scroll', this.onScroll)
  },
}
</script>

<style>
.bgBlur {
  background: rgb(0, 0, 0, 0.7);
  backdrop-filter: blur(2px);
  -webkit-backdrop-filter: blur(2px);
  transition: 1000ms;
}

.bgBlur a {
  color: white;
}

#nav {
  transition: 1000ms;
  backdrop-filter: blur(2px);
  -webkit-backdrop-filter: blur(2px);
}

.hideNav {
  transform: translateX(-100%);
}

.showNav {
  transform: translateX(0);
}

.links .nuxt-link-exact-active {
  border-bottom: 3px #fff solid;
}

.links a:hover {
  border-radius: 3px;
}
</style>