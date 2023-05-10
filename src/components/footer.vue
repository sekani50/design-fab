<!-- eslint-disable -->
<template>
  <div class="bg-zinc-900 w-full p-6 text-white text-sm sm:text-lg">
    <div class="flex flex-col sm:flex-row justify-around space-y-3">

      <div class="flex flex-col space-y-3 justify-start">
        <div class="sm:h-10 sm:w-10 h-8 w-8">
        
            <img src="@/assets/images/def.png" alt="wht" />
          
        </div>
        
        <p class="capitalize underline">Contact Info</p>
        <div class="flex space-x-2 items-center group">
          <span class="" v-html="images.tel"></span>
          <p class="">08104149992</p>
        </div>
        <div class="flex space-x-2 items-center group">
          <span class="" v-html="images.email"></span>
          <p class="">official.designfab@gmail.com</p>
        </div>
      </div>
      <div class="flex flex-col space-y-3 justify-start">
        <p class="capitalize underline">Location address</p>
        <p>No. 4 manomi street, Aiport Road, Mando, Kaduna, Nigeria</p>
      </div>
   
      <div class="flex items-center space-x-2">
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
  name: "Footer",

  data() {
    return {
      images: assets,
    };
  },
};
</script>

<style scoped>
/* eslint-disable */
</style>
