<template>
  <div class=" 2xl:ml-[230px] lg:ml-40 sm:mr-6 w-12 sm:-ml-2 md:ml-44 xmd:ml-auto  flex flex-col  ">
    <button
      class="mb-2 p-2 sm:p-3 2xl:p-[15px] 2xl:ml-[90px] lg:-ml-14 w-16 -ml-4 md:-ml-81 sm:ml-2  rounded-full items-center flex     cursor-pointer justify-center hover:duration-200  hover:bg-134 ">
      <img class="h-8 " src="../assets/twitter_white.svg">

    </button>
    <div class="   2xl:ml-24 lg:-ml-14 md:ml-0 xmd:ml-24  flex  flex-col  ">

      <a href="/">
        <button
          class="  sm:pl-7  xmd:-ml-24 lg:-ml-0 sm:-ml-1 lg:p-2.5  md:w-150 w-150 lg:w-150  sm:w-20 rounded-30 items-center flex    text-#e7e9ea h-50 mb-1 font-bold font-sans text-18 cursor-pointer hover:duration-200 hover:bg-134">
          <img class="pr-5 h-7 hidden 2xl:block md:block sm:hidden" src="../assets/twitter_hashtag.svg">
          <p class="hidden lg:block md:hidden ">Keşfet</p>
          <img class="pr-[25px] h-6 hidden md:hidden  sm:block" src="../assets/twitter_search.svg">
        </button>

      </a>
      <a href="/">
        <button
          class="sm:pl-7 lg:-ml-0 xmd:-ml-24 sm:-ml-1 lg:p-2.5 md:w-150 w-150 lg:w-150  sm:w-20 rounded-full items-center flex    text-#e7e9ea h-50 mb-1 font-bold font-sans text-18 cursor-pointer hover:duration-200 hover:bg-134">
          <img class=" pr-5 " src="../assets/twitter_setting.svg">
          <p class=" hidden lg:block md:hidden ">Ayarlar</p>
        </button>

      </a>




    </div>
  </div>
</template>

<script>
export default {
  name: 'Menu'
}
</script>

