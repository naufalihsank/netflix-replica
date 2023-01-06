<template>
  <div class="ml-[4%] max-h-[200px]">
    <h1 class="flex font-netflixsans text-[#e5e5e5] hover:text-white leading-[1.25vw] font-medium text-[1.4vw] mb-5 hover:cursor-pointer items-end group">
      {{ title }}
      <button class="text-[#54b9c5] text-[.9vw] leading-[.8vw] font-bold ml-3 trans-explore opacity-0 group-hover:opacity-100 w-auto text-start">
        Explore All >
      </button>
    </h1>
    <swiper ref="mySwiper">
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <swiper-slide><BaseVideoCard /></swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss" scoped>
.swiper-slide {
  @apply max-w-[15vw];
}
.trans-explore {
  transition: opacity 1s, transform .75s;
}
</style>
