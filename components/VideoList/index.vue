<template>
  <div class="ml-[4%] max-h-[200px]">
    <h1 class="font-netflixsans text-[#e5e5e5] leading-[1.25vw] font-medium text-[1.4vw] mb-5 hover:cursor-pointer">
      {{ title }}
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
</style>
