<!-- eslint-disable -->
<template>
  <div class="w-full mt-[60px] sm:mt-[68px] space-y-[5%] mx-auto p-6 text-zinc-900">

    <div class="space-y-[5%] sm:p-6 p-3 font-medium rounded-md w-full sm:w-[60%] bg-[#3C9DC5] text-zinc-900 mx-auto">
        <div class="flex flex-col space-y-3 justify-start">
        <p class="capitalize underline">Location address</p>
        <div class="flex space-x-2 items-center">
          <div v-html="images.loc"></div>
        <p>No. 4 manomi street, Kaduna, Nigeria</p>

        </div>
      </div>
      <div class="flex flex-col space-y-3 justify-start">
        <p class="capitalize underline">Contact Info</p>
        <div class="flex space-x-2 items-center group">
          <span class="sm:h-6 sm:w-6 h-4 w-4">
            <img src="@/assets/tel.svg" alt="wht" />
          </span>
          <p class="">08104149992</p>
        </div>
        <div class="flex space-x-2 items-center group">
            <span class="sm:h-6 sm:w-6 h-4 w-4">
            <img src="@/assets/email.svg" alt="wht" />
          </span>
          <p class="">official.designfab@gmail.com</p>
        </div>
      </div>
      <div class="flex items-center justify-start space-x-2">
        <div class="sm:h-8 sm:w-8 h-6 w-6">
          <a href="">
            <img src="@/assets/whatsapp.svg" alt="wht" />
          </a>
        </div>
        <div class="sm:h-8 sm:w-8 h-6 w-6">
          <a href="https://instagram.com/designfab_?igshid=ZDdkNTZiNTM=">
            <img src="@/assets/insta.svg" alt="inst" />
          </a>
        </div>
        <div class="sm:h-8 sm:w-8 h-6 w-6">
          <a href="https://www.facebook.com/profile.php?id=100090622029660&mibextid=ZbWKwL">
            <img src="@/assets/fb.svg" alt="fb" />
          </a>
        </div>
      </div>
      </div>
  
  </div>
</template>
<!--eslint-disable-->
<script>
/* eslint-disable */
import { assets } from "@/assets/svgimages.js";
export default {
  name: "ContactCont",
  components: {},

  data() {
    return {
        email:"",
        message: "",
        images: assets,
    };
  },
};
</script>

<style scoped>
/* eslint-disable */

.input-field {
  @apply border bg-white text-zinc-700 border-zinc-700 rounded-md focus:outline-none w-full h-10 sm:h-14 px-2;
}

</style>
