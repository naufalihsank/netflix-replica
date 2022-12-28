<template>
  <div
    :class="{
      'flex fixed align-middle px-[4%] text-white items-center justify-between w-full z-[2] bg-[#0e0e0e] transition duration-500': true,
      'bg-transparent': position[1] === 0
    }"
  >
    <div class="flex items-center">
      <a href="/" class="mr-9">
        <img src="@/assets/images/navbar-icon.png" alt="Netflix Icon" width="92" height="30">
      </a>
      <ul class="flex gap-[18px] font-netflixsans text-sm text-[#e5e5e5]">
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">Home</li>
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">TV Shows</li>
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">Movies</li>
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">New & Popular</li>
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">My List</li>
        <li class="transition duration-300 hover:cursor-pointer hover:opacity-50">Browse by Languages</li>
      </ul>
    </div>
    <div class="flex">
      <img src="@/assets/icons/search.svg" alt="Search" width="24" height="24" class="mr-5 hover:cursor-pointer">
      <img src="@/assets/icons/notification.svg" alt="Notification" width="24" height="24" class="mr-3 hover:cursor-pointer">
      <div class="flex group items-center hover:cursor-pointer">
        <div class="w-[32px] h-[32px] bg-white rounded-md mr-3"></div>
        <img src="@/assets/icons/arrow-down.png" alt="Arrow" width="10" height="10" class="hidden lg:block group-hover:rotate-180 transition duration-300">
      </div>
    </div>
  </div>
</template>

<script>
import windowScrollPosition from '@@/utils/window-scroll-position'

export default {
  mixins: [windowScrollPosition('position')]
}
</script>
