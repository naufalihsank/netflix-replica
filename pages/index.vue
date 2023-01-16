<template>
  <div class="text-white pb-[50px]">
    <HomePlayer />
    <VideoList title="Trending Now" class="mt-[2%] 2xl:mt-[4%]" />
    <VideoList title="Recently Added" class="mt-[2%] 2xl:mt-[4%]" />
    <VideoList title="Marvel Studios" class="mt-[2%] 2xl:mt-[4%]" />
    <!-- <div class="grid grid-cols-6 gap-3">
      <div v-for="i in 18" :key="i" class="group hover:scale-[1.8] h-[200px] hover:delay-1000 transition">
        <div class="w-[200px] h-full bg-red-400 group-hover:delay-1000 group-hover:h-0">
        </div>
        <div class="w-[200px] group-hover:h-1/2 bg-blue-400 group-hover:delay-1000 h-0">
        </div>
        <div class="w-[200px] h-0 group-hover:h-1/2 bg-green-400 group-hover:delay-1000">
        </div>
      </div>
    </div> -->
    <div class="grid grid-flow-col gap-3">
      <div v-for="i in 18" :key="i" class="group hover:scale-[1.8] h-[200px] hover:delay-1000 transition">
        <div class="w-[200px] h-full bg-red-400 group-hover:delay-1000 group-hover:h-0">
        </div>
        <div class="w-[200px] group-hover:h-1/2 bg-blue-400 group-hover:delay-1000 h-0">
        </div>
        <div class="w-[200px] h-0 group-hover:h-1/2 bg-green-400 group-hover:delay-1000">
        </div>
      </div>
    </div>
    <div class="grid grid-flow-col gap-3 mt-[2%] 2xl:mt-[4%]">
      <div v-for="i in 18" :key="i" class="group hover:scale-[1.8] h-[200px] hover:delay-1000 transition">
        <div class="w-[200px] h-full bg-red-400 group-hover:delay-1000 group-hover:h-0">
        </div>
        <div class="w-[200px] group-hover:h-1/2 bg-blue-400 group-hover:delay-1000 h-0">
        </div>
        <div class="w-[200px] h-0 group-hover:h-1/2 bg-green-400 group-hover:delay-1000">
        </div>
      </div>
    </div>
    <div class="grid grid-flow-col gap-3 mt-[2%] 2xl:mt-[4%]">
      <div v-for="i in 18" :key="i" class="group hover:scale-[1.8] h-[200px] hover:delay-1000 transition">
        <div class="w-[200px] h-full bg-red-400 group-hover:delay-1000 group-hover:h-0">
        </div>
        <div class="w-[200px] group-hover:h-1/2 bg-blue-400 group-hover:delay-1000 h-0">
        </div>
        <div class="w-[200px] h-0 group-hover:h-1/2 bg-green-400 group-hover:delay-1000">
        </div>
      </div>
    </div>
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
