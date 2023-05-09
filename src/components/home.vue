<!-- eslint-disable -->
<template>
  <div class="w-full">
    <HeroPage />
    <ExploreService
     
    />
  </div>
</template>
<!--eslint-disable-->
<script>
/* eslint-disable */

import HeroPage from "@/components/banners/heropage.vue";
import ExploreService from "@/components/products/service.vue";

export default {
  name: "HomePage",
  components: {
    HeroPage,
    ExploreService,
  },

  data() {
    return {
   
    };
  },

  async mounted() {

  },
  methods: {},
};
</script>

<style scoped>
/* eslint-disable */
</style>
