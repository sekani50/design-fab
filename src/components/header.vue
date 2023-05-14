<!-- eslint-disable -->
<template>
  <div
    class="h-fit w-full sm:w-full text-white text-sm sm:text-lg absolute inset-0 bg-black bg-opacity-70 shadow-lg z-50"
  >
 <div class="px-[5%] sm:py-4 py-3 w-full flex items-center justify-between">
  <router-link to="/">
    <div class="flex items-center space-x-2">
      <!--

        <div class="rounded-full h-6 w-6 sm:h-8 sm:w-8 border  border-zinc-800">
      <img src="@/assets/images/logoB.png" class="ml-[2px] mt-[2px] rounded-full w-full h-full object-cover" alt="l"/>

      </div>
      -->
      <div class="sm:h-10 sm:w-10 h-8 w-8">
        
        <img src="@/assets/images/def.png" alt="wht" />
      
    </div>
   <p class="collectio text-white text-2xl sm:text-4xl font-medium">DesignFab</p>
  
  </div>
  </router-link>
 
  <div class="hidden text-white  md:flex items-center space-x-10">
    <router-link to="/">
      <button 
      :class="currentRoute === 'MainPage' ? 'text-[#3C9DC5]' :'text-white' " 
      class="navs relative hover:text-[#3C9DC5] ">Home</button>
    </router-link>
    <router-link to="/">
      <button class="navs relative hover:text-[#3C9DC5]">Projects</button>
    </router-link>
    <router-link to="/contact">
      <button 
      :class="currentRoute === 'ContactView' ? 'text-[#3C9DC5]' :'text-white' " 
      class="navs relative hover:text-[#3C9DC5]">Contact</button>
    </router-link>
   
   
    
    </div>
    <div
    @click="menuClick"
     class="md:hidden" v-html="images.menu"></div>

 </div>

 
 <div
 @click.self="menuClick"
 :class="isVisible ? 'block' : 'hidden' "
  class="let swipeIn bg-opacity-50 bg-[#000] fixed w-full h-full overflow-hidden inset-0">
    <div class=" absolute right-0 top-0 bg-[#FFFFFF] w-1/3 h-full">
      <div class="flex flex-col mr-[4%] sm:mr-[9%] justify-end items-end p-[18px]">
      <div
      @click="menuClick"
      class=" " v-html="images.close"></div>

      </div>
      <div class="flex flex-col w-full text-zinc-900 justify-start space-y-3 px-6">
        <router-link to="/">Home</router-link>
        <router-link to="/services">Projects</router-link>
        <router-link to="/contact">Contact</router-link>
       
       
       
        

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
  name: "HeaderSect",

  data() {
    return {
      images:assets,
      isVisible: false
      
    };
  },
  computed: {
    currentRoute () {
     // console.log(this.$route.name)
      return this.$route.name
    }

  },
  methods: {
    menuClick() {
      this.isVisible = !this.isVisible;
    }
  }
};
</script>

<style scoped>
/* eslint-disable */
.show {
  @apply sm:block
}
.hide {
  @apply sm:hidden
}
.text {
    @apply text-zinc-700 bg-black bg-opacity-10 sm:text-lg text-sm lg:text-[15px] p-3 rounded-l-none sm:rounded-l-none   sm:rounded-r-lg rounded-md sm:rounded-lg border-l-4 border-l-[#3452FF];
}
</style>
