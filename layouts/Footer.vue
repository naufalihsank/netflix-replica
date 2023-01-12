<template>
  <div class="flex flex-col mx-auto mt-20 font-netflixsans max-w-[980px] text-[#808080]">
    <!-- Social Media -->
    <div class="flex gap-10 mb-[10px]">
      <img src="@/assets/icons/facebook.svg" alt="Facebook Logo" class="hover:cursor-pointer">
      <img src="@/assets/icons/instagram.svg" alt="Instagram Logo" class="hover:cursor-pointer">
      <img src="@/assets/icons/twitter.svg" alt="Twitter Logo" class="hover:cursor-pointer">
      <img src="@/assets/icons/youtube.svg" alt="Youtube Logo" class="hover:cursor-pointer">
    </div>

    <!-- Information List -->
    <div class="grid grid-cols-2 md:grid-cols-4 gap-y-4 text-[13px] mb-[14px]">
      <a v-for="info in infoList" :key="info" class="hover:cursor-pointer hover:underline">
        {{ info }}
      </a>
    </div>

    <!-- Service Code -->
    <button class="self-start p-[6.5px] border border-[#808080] text-[13px] mb-5 hover:text-white">
      Service Code
    </button>

    <!-- Copyright -->
    <span class="text-[11px] mb-[15px]">
      © 1997-2023 Netflix, Inc.‎
    </span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      infoList: [
        'Audio Description',
        'Help Center',
        'Gift Cards',
        'Media Center',
        'Investor Relations',
        'Jobs',
        'Terms of Use',
        'Privacy',
        'Legal Notices',
        'Cookie Preferences',
        'Corporate Information',
        'Contact Us'
      ]
    }
  }
}
</script>
