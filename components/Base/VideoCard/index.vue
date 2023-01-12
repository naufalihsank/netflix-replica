<template>
  <div
    class="flex flex-col w-[15vw] transition hover:scale-[1.35] relative group-hover:z-10 duration-300 group hover:cursor-pointer hover:delay-700"
    @mouseover="playVideo(true)"
    @mouseleave="playVideo(false)"
  >
    <!-- Video Section-->
    <img src="@/assets/images/avengers.webp" alt="Video Cover" class="h-full group-hover:h-0 group-hover:delay-700 rounded-[0.2vw]">
    <iframe :src="src" frameborder="0" allowfullscreen class="group-hover:h-1/2 rounded-[0.2vw] group-hover:delay-700 h-0 opacity-0 group-hover:opacity-100"></iframe>
    <!-- Button Section -->
    <div class="scale-y-0 opacity-0 h-0 group-hover:h-1/2 group-hover:scale-y-100 group-hover:opacity-100 bg-[#111111] transition-opacity duration-300 group-hover:delay-700 ease-in-out flex flex-col p-4 group-hover:shadow-xl">
      <!-- Action Button -->
      <div class="flex justify-between">
        <div class="flex items-start">
          <button class="rounded-full w-[27px] h-[27px] mr-[6px] bg-white hover:bg-[#e6e6e6] flex justify-center items-center">
            <img src="@/assets/icons/play.svg" alt="Replay Button" class="w-[18px]">
          </button>
          <button class="border border-white rounded-full w-[27px] h-[27px] mr-[6px] bg-[#181818] hover:bg-[#ffffff1a] flex justify-center items-center">
            <img src="@/assets/icons/plus.svg" alt="Plus Button" class="w-[18px]">
          </button>
          <button class="border border-white rounded-full w-[27px] h-[27px] bg-[#181818] hover:bg-[#ffffff1a] flex justify-center items-center">
            <img src="@/assets/icons/thumb-up.svg" alt="Like Button" class="w-[18px]">
          </button>
        </div>
        <button class="border border-white rounded-full w-[27px] h-[27px] bg-[#181818] hover:bg-[#ffffff1a] flex justify-center items-center">
          <img src="@/assets/icons/chevron-down.svg" alt="Info Button" class="w-[18px]">
        </button>
      </div>

      <!-- Information -->
      <div class="flex mt-3 text-xs items-center font-netflixsans">
        <span class="text-[#46d369] font-medium mr-2">
          99% Match
        </span>
        <span class="border border-[#ffffff66] px-[6.4px] mr-1">
          13+
        </span>
        <span class="border border-[#ffffff66] px-[6.4px] text-[8px]">
          HD
        </span>
      </div>

      <!-- Category -->
      <div class="flex mt-3 text-xs items-center font-netflixsans">
        <span class="font-medium">
          Feel-Good
        </span>
        <svg height="4" width="4" class="min-w-[2px] mt-[2px] mx-[5px]">
          <circle cx="2" cy="2" r="2" fill="#646464" />
        </svg>
        <span>
          Goofy
        </span>
        <svg height="4" width="4" class="min-w-[2px] mt-[2px] mx-[5px]">
          <circle cx="2" cy="2" r="2" fill="#646464" />
        </svg>
        <span>
          Superhero
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      videoSource: 'https://www.youtube.com/embed/TcMBFSGVi1c',
      videoParams: 'rel=0&modestbranding=0&autohide=1&mute=1&showinfo=0&controls=0&autoplay=0'
    }
  },
  computed: {
    src() {
      return `${this.videoSource}?${this.videoParams}`
    }
  },
  methods: {
    playVideo(value) {
      const isPlay = value ? '1' : '0'
      this.videoParams = `rel=0&modestbranding=1&autohide=1&mute=1&showinfo=0&controls=0&autoplay=${isPlay}`
    }
  }
}
</script>
