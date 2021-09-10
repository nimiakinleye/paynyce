<template>
  <div>
    <div class="contact">
      <div data-aos="fade-up-right" class="contact_information">
        <div>
          <h2>Let's Talk</h2>
          <p>
            Feel we need to fix something? Need enlightenment on any of our
            service? Have issues and haven’t gotten a reply from the business
            involved? Have issues using any of our platforms? Just send us a
            message
          </p>
        </div>
        <div class="contact_media">
          <div class="contact_medium">
            <svg
              viewBox="0 0 512 512"
              style="enable-background: new 0 0 512 512"
            >
              <g>
                <g>
                  <path
                    d="M256,0C161.896,0,85.333,76.563,85.333,170.667c0,28.25,7.063,56.26,20.49,81.104L246.667,506.5    c1.875,3.396,5.448,5.5,9.333,5.5s7.458-2.104,9.333-5.5l140.896-254.813c13.375-24.76,20.438-52.771,20.438-81.021    C426.667,76.563,350.104,0,256,0z M256,256c-47.052,0-85.333-38.281-85.333-85.333c0-47.052,38.281-85.333,85.333-85.333    s85.333,38.281,85.333,85.333C341.333,217.719,303.052,256,256,256z"
                  />
                </g>
              </g>
            </svg>
            <p>Milky Way</p>
          </div>
          <div class="contact_medium">
            <svg
              viewBox="0 0 513.64 513.64"
              style="enable-background: new 0 0 513.64 513.64"
            >
              <g>
                <g>
                  <path
                    d="M499.66,376.96l-71.68-71.68c-25.6-25.6-69.12-15.359-79.36,17.92c-7.68,23.041-33.28,35.841-56.32,30.72    c-51.2-12.8-120.32-79.36-133.12-133.12c-7.68-23.041,7.68-48.641,30.72-56.32c33.28-10.24,43.52-53.76,17.92-79.36l-71.68-71.68    c-20.48-17.92-51.2-17.92-69.12,0l-48.64,48.64c-48.64,51.2,5.12,186.88,125.44,307.2c120.32,120.32,256,176.641,307.2,125.44    l48.64-48.64C517.581,425.6,517.581,394.88,499.66,376.96z"
                  />
                </g>
              </g>
            </svg>
            <p>+234 9067 891 012</p>
          </div>
        </div>
      </div>
      <div data-aos="fade-up-left" class="contact_form">
        <form @submit.prevent="submit">
          <div class="md:grid grid-cols-2 gap-x-12">
            <div class="input">
              <label for="first_name">First Name*</label>
              <input name="first_name" type="text" />
            </div>
            <div class="input">
              <label for="last_name">Last Name*</label>
              <input name="last_name" type="text" />
            </div>
            <div class="input">
              <label for="email">Email Address*</label>
              <input name="email" type="text" />
            </div>
            <div class="input">
              <label for="phone">Telephone Number*</label>
              <input name="phone" type="text" />
            </div>
          </div>
          <div class="input">
            <label for="message">Message</label>
            <textarea
              name="message"
              id=""
              placeholder="Write your message..."
            ></textarea>
          </div>
          <div class="button">
            <button class="my-bg" type="submit">Send Message</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        first_name: '',
        last_name: '',
        mail: '',
        phone: '',
        message: '',
      },
    }
  },
}
</script>

<style>
.contact {
  @apply flex
  flex-col-reverse
  lg:grid
  grid-cols-12
  gap-x-12
  px-12;
}

.contact .contact_information {
  @apply col-start-1
  col-end-5
  bg-purple-900
  px-10
  py-5
  lg:rounded-lg
  text-white
  mt-6
  lg:mt-0;
  background-image: url('~/assets/contact_bg.svg');
  background-repeat: no-repeat;
  background-position: bottom right;
}

.contact .contact_information h2 {
  @apply font-semibold
  text-2xl
  mb-3;
}

.contact .contact_information p {
  @apply font-light;
}

.contact .contact_form {
  @apply col-start-5 col-end-13
  px-10;
}

.contact .contact_media .contact_medium {
  @apply flex
  items-center
  my-12;
}

.contact_media .contact_medium svg {
  @apply w-5
  mr-2
  fill-current;
  color: #ff350d;
}

.contact_social {
  @apply flex items-center;
}

.contact_social a svg {
  @apply w-10
  mr-5
  text-white
  fill-current
  p-1
  hover:bg-white
  hover:text-gray-700
  rounded-lg;
}

.contact_form .input {
  @apply flex
  flex-col
  my-3;
}

.contact_form .input label {
  @apply text-gray-500
  font-normal
  text-sm
  mb-3;
}

.contact_form input,
.contact_form textarea {
  @apply bg-gray-200
  bg-opacity-30
  outline-none
  rounded-md
  h-10
  p-2;
}

.contact_form textarea {
  @apply h-24;
}

.input h1 {
  color: #374151;
  @apply font-bold
  text-xl
  mb-3;
}

form button {
  @apply p-2
  px-10
  text-white
  font-normal
  rounded-lg
  text-right;
}

form button:active {
  @apply bg-yellow-100
  text-gray-600;
}
</style>