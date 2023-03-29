<template>
  <div
    class=" w-600 lg:w-600 md:w-600 xmd:w-600 sm:w-600 -mt-1 ml-80 2xl:ml-72 lg:ml-36 xmd:mr-40  md:-ml-16 sm:ml-0 md:mr-auto lg:mr-4  justify-between border-solid border-thin border-x-47  ">

    <div class="flex flex-row items-center pl-4 justify-between">
      <div class="w-11/12 flex flex-row">
        <div class="h-11 flex items-center justify-center cursor-pointer mt-2 rounded-tl-30 rounded-bl-30 bg-#202327">
          <img class=" mr-4 h-4 ml-4 " src="../assets/twitter_search.svg" alt="" />
        </div>

        <input type="search" name="search-input" id="search-input"
          class="w-5/6  h-11 pl-4 text-15 rounded-30  mt-2 rounded-tl-none rounded-bl-none bg-#202327"
          placeholder="Twitter'da Ara" />
      </div>
      <div class="cursor-pointer mb-1 p-2  bg-transparent mr-2 mt-4 rounded-3xl hover:duration-200 hover:bg-0,25">
        <img class="h-5" src="../assets/twitter_setting.svg" alt="">
      </div>


    </div>

    <div class="flex flex-col  pl-3 text-white">
      <span class="flex flex-col mt-2.5 text-231 text-20 mb-2 font-extrabold font-twitter"> {{ newTitle }}</span>
    </div>


    <button v-for="tab in tabs" class="w-full flex whitespace-nowrap justify-between hover:bg-134 pt-2 pb-2  ">
      <div class="flex flex-col pl-3  whitespace-nowrap">
        <p class="text-#71767b text-13 cursor-pointer whitespace-nowrap contrast-150 font-twitter flex ">{{ tab.title }}
          <img
            class="h-5 ml-auto xmd:mr-8 2xl:ml-96 md:ml-96 sm:ml-56 sm:left-auto  xmd:ml-96 whitespace-nowrap lg:whitespace-nowrap sm:whitespace-nowrap md:whitespace-nowrap xmd:whitespace-nowrap   "
            src="../assets/abaout.svg" alt="">
        </p>
        <p class="text-231  text-15 font-bold font-twitter  whitespace-nowrap text-left">{{ tab.handle }} </p>
        <p class="text-#71767b text-13 cursor-pointer whitespace-nowrap contrast-150 font-twitter text-left"> {{ tab.name
        }}</p>

      </div>

    </button>
    <button class="w-full flex justify-between hover:bg-134 pt-2 pb-2 ">
      <span class="text-240  text-15 font-twitter text-left p-px pl-4"> {{ more }} </span>

    </button>






    <div
      class=" top-3/4 mt-40 w-full lg:max-full sm:w-full md:w-full  left-0 h-72 2xl:h-72 md:h-72 sm:h-72 lg:h-72 smd:h-72 xmd:h-72  flex fixed   bg-cyan-600  shadow-lg shadow-gray-400/50 ">

      <h1
        class="top-2 2xl:ml-auto 2xl:left-36 lg:ml-56 md:ml-10 xmd:-ml-auto left-52 smd:left-36  text-2xl relative text-255 contrast-200 font-bold font-twitter flex xmd:hidden md:block sm:hidden smd:block whitespace-nowrap">
        {{ h1 }}</h1>

      <p
        class="text-255 font-normal  right-11 2xl:-left-auto top-9 smd:-ml-16 text-md relative font-twitter  hidden  md:block 2xl:block  xmd:hidden  smd:block whitespace-nowrap">
        {{ twitterUser }}</p>


      <button
        class="bg-transparent text-white font-bold justify-center text-15 ml-auto md:ml-auto   mt-4 h-9 w-24 lg:w-24 sm:w-85 xmd:ml-4 xmd:w-96 smd:w-24 smd:ml-auto border-solid border whitespace-nowrapp border-0.35  rounded-30 cursor-pointer hover:bg-0,25 hover:duration-200 font-twitter  whitespace-nowrap sm:ml-5 ">{{
          login }}</button>
      <button
        class="text-15 font-bold justify-center border border-solid border-0.35 ml-2.5 mr-80 2xl:mr-96 md:mr-16 sm:mr-4 xmd:w-96 xmd:mr-4 xmd:ml-2 smd:mr-48 smd:w-20 sm:w-85 mt-4 h-9 lg:w-24 bg-white text-black whitespace-nowrap font-twitter rounded-30 cursor-pointer ">{{
          register }}</button>



    </div>
  </div>
</template>

<script >
export default {
  name: "Feed",
  data() {
    return {

      tabs: [
        { title: 'Türkiye tarihinde gündemde', handle: '#ŞAMPİYON TAKIM', name: '200,1 B Tweet' },
        { title: 'Türkiye tarihinde gündemde', handle: '#FENERBAHÇE', name: '200,1 B Tweet' },
        { title: 'Türkiye tarihinde gündemde', handle: '#GALATASARAY', name: '120,1 B Tweet' },
        { title: 'Türkiye tarihinde gündemde', handle: '#BEŞİKTAŞ', name: '180,1 B Tweet' },
        { title: 'Türkiye tarihinde gündemde', handle: '#TRABZONSPOR', name: '20,1 B Tweet' },




      ],

      newTitle: "İlgini çekebilecek gündemler",
      h1: 'Olup bitenleri kaçırma',
      twitterUser: 'İlk öğrenen Twitter kullanıcıları olacak.',
      login: 'Giriş Yap',
      register: 'Kaydol',
      more: 'Daha Fazlası için'


    }
  }
};
</script>

