<template>
  <lite-youtube videoid="TcMBFSGVi1c" :params="videoParams" class="w-full aspect-auto max-w-full max-h-screen relative hover:cursor-default font-netflixsans">
    <div class="absolute bottom-[35%] pl-[4%] z-2">
      <p class="max-w-[518px] text-[1.1vw]">
        Whatever it takes. Watch the brand-new trailer for Marvel Studios’ Avengers: Endgame. In theaters April 26.
      </p>
      <div class="flex mt-[1.5vw]">
        <button class="flex bg-white text-black text-lg pl-[22px] pr-[26px] py-[9px] gap-3 rounded-[4px] items-center font-bold mr-[10px] hover:opacity-80">
          <img src="@/assets/icons/play.svg" alt="Play Button">
          Play
        </button>
        <button class="flex bg-[#4d5155] text-white text-lg pl-[22px] pr-[26px] py-[9px] gap-3 rounded-[4px] items-center font-bold hover:opacity-80">
          <img src="@/assets/icons/info-circle.svg" alt="Info Button">
          More Info
        </button>
      </div>
    </div>
    <div class="flex absolute bottom-[33.5%] right-0 z-2">
      <button class="border border-[#ffffffb3] rounded-full p-2 mr-[15.8px] hover:bg-[#ffffff1a]">
        <img src="@/assets/icons/replay.svg" alt="Replay Button" width="20">
      </button>
      <div class="bg-[#33333399] pl-[11.5px] pr-[50.4px] py-[7.2px] text-white border-l-4 leading-5">
        13+
      </div>
    </div>
  </lite-youtube>
</template>

<script>
export default {
  data() {
    return {
      videoParams: 'rel=0&modestbranding=1&autohide=1&mute=1&showinfo=0&controls=0&autoplay=1'
    }
  }
}
</script>
