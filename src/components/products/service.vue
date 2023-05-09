<!-- eslint-disable -->
<template>
  <div class="collectio w-full mt-[-25px] sm:mt-0 space-y-[5%]">
    <div class="flex w-full justify-center items-center space-x-2">
      <span class="h-[2px] w-16 sm:w-24 bg-[#3C9DC5] relative">
        <span
          class="absolute w-[6px] h-[6px] transform rotate-45 bg-[#3C9DC5] right-0 top-[-2px]"
        ></span>
      </span>
      <P class="uppercase font-semibold text-[#3C9DC5] sm:text-2xl text-lg"
        >Design Fab_</P
      >
      <span class="h-[2px] w-16 sm:w-24 bg-[#3C9DC5] relative">
        <span
          class="absolute w-[6px] h-[6px] transform rotate-45 bg-[#3C9DC5] left-0 top-[-2px]"
        ></span>
      </span>
    </div>

    <div class="p-4 sm:p-8 text-start">
      <b>DesignFab</b> is an
      <b><i>innovative engineering design, simulation, and fabrication</i></b>
      company that offers technical expertise to its clients. We specialize in
      providing customized solutions to meet the specific needs of our
      customers, and our team of skilled engineers and designers is dedicated to
      providing quality services to help our clients improve the quality of
      their products and services. <br />At <b>DesignFab</b>, we understand that
      time-to-market is critical for our customers, which is why we offer
      simulation services to help our clients test and validate their designs
      before fabrication. This reduces the time it takes to bring products to
      market, helping our customers stay ahead of their competition. Our
      fabrication services help our customers save costs on manufacturing and
      importation while still ensuring high-quality products. We use quality
      control measures to ensure that our products meet the required quality
      standards and that our customers are satisfied with the products they
      receive. <br />
      At <b>DesignFab</b>, we pride ourselves on our commitment to quality and
      customer satisfaction. We believe that our technical expertise, customized
      solutions, faster time-to-market, cost savings, and quality assurance
      measures set us apart from our competitors and make us the go-to
      engineering design, simulation, and fabrication company for clients in
      various industries.
    </div>

    <div
      class="p-2 sm:p-6 bg-black bg-opacity-70  relative sm:py-8 py-6 w-full h-fit"
    >
      <div class="absolute inset-0 w-full h-full -z-10">
        <img
          class="w-full h-full object-cover"
          src="@/assets/images/fabs1.jpg"
          alt=""
        />
      </div>

      <p
        class="text-[#3C9DC5] uppercase text-lg font-bold sm:text-2xl flex items-center space-x-2"
      >
        <span class="text-4xl">+</span> <span>What we do</span>
      </p>

      <div class="mx-auto grid grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
        <div
          class="text-zinc-900 text-center w-full sm:p-6 p-4 space-y-2 bg-white flex flex-col justify-center items-center shadow-lg rounded-lg"
        >
          <div class="w-12 h-12 sm:w-16 sm:h-16">
            <img class="w-full h-full" src="@/assets/images/solid.png" alt="" />
          </div>
          <div class="space-y-2">
            <p class="uppercase font-semibold">engineering simulation</p>

            <div>
              We have experts specializes in providing high-quality engineering
              simulation solutions tailored to your specific needs. With
              advanced software and years of experience, we can simulate
              everything from fluid dynamics to structural analysis, helping you
              make informed design decisions and improve your products.
            </div>
          </div>
        </div>

        <div
          class="text-gray-900 text-center w-full sm:p-6 p-4 space-y-2 bg-white flex flex-col justify-center items-center shadow-lg rounded-lg"
        >
          <div class="w-12 h-12 sm:w-16 sm:h-16">
            <img
              class="w-full h-full"
              src="@/assets/images/design.png"
              alt=""
            />
          </div>
          <div class="space-y-2">
            <p class="uppercase font-semibold">engineering design</p>

            <div>
              We have experienced engineers dedicated to providing top-notch
              solutions tailored to meet your unique needs. From concept to
              completion, we'll work closely with you to ensure that your
              project is completed on time, on budget, and to your satisfaction
            </div>
          </div>
        </div>

        <div
          class="text-gray-900 text-center w-full sm:p-6 p-4 space-y-2 bg-white flex flex-col justify-center items-center shadow-lg rounded-lg"
        >
          <div class="w-12 h-12 sm:w-16 sm:h-16">
            <img
              class="w-full h-full"
              src="@/assets/images/fabricate.png"
              alt=""
            />
          </div>
          <div>
            <p class="uppercase font-semibold">fabrication</p>
            <div>
              We specialize in providing customized fabrication solutions
              tailored to your unique needs. From welding to machining, we have
              the tools and expertise to fabricate everything from complex
              assemblies to simple components. Whether you need a prototype or a
              full production run, we'll work closely with you to ensure that
              your project is completed on time and to your satisfaction.
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="w-8 h-8 bg-none"></div>
  </div>
</template>
<!--eslint-disable-->
<script>
/* eslint-disable */
import ProductWidgets from "./widget.vue";

import { mapGetters, mapActions } from "vuex";

export default {
  name: "ExploreService",
  props: [],
  components: {},
  data() {
    return {
      image: null,
      isminiDetail: false,
      name: "",
      description: "",
      cats: "",
      price: "",
      idx: "",
    };
  },
  methods: {
    ...mapActions(["updateCategory"]),
    showMiniDetail() {},
    toggleminiDetails() {},
    sendMessage() {},
    showMore() {},
  },
};
</script>

<style scoped>
/* eslint-disable */
.grids {
  @apply mx-auto grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-2 sm:gap-[3rem] lg:gap-[70px] text-zinc-900;
}
</style>
