<template>
  <div class="text-white pb-[50px]">
    <HomePlayer />
    <VideoList title="Trending Now" class="mt-[4%]" />
    <VideoList title="Recently Added" class="mt-[2%]" />
    <VideoList title="Marvel Studios" class="mt-[2%]" />
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: 'Netlix Jawa Barat'
    }
  }
}
</script>
