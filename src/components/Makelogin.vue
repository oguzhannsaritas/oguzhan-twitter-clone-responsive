<template>
    <div
        class="w-80 h-304 md:w-85 md:h-304 2xl:h-[305px] 2xl:w-85   2xl:flex  pr-6 pl-1 2xl:mr-350 xmd:ml-5 md:mr-48  mt-2.5 xmd:hidden md:flex sm:hidden  flex-col rounded-2xl sticky border-47 border-solid border-thin">
        <span class="mt-2  text-231 font-bold ml-3 mb-2   text-20 font-twitter   "> {{ twitterNew }}</span>
        <span class="text-#71767b pl-2 text-13 leading-[15px]   pb-4  contrast-150 ">
            {{ user }}
        </span>
        <div class=" flex flex-col  2xl:pr-4   pl-4 md:pl-2 pb-4  md:pb-5 items-center ">
            <button
                class="w-300 h-38  rounded-30 mb-3 pb-1 flex text-14  items-center  tracking-wide justify-center font-medium text-#202124 bg-255 cursor-pointer hover:bg-230">
                <span class="font-twitter  contrast-100 "> <img class="-ml-8  -mb-5 " src="../assets/google.svg" alt=""> {{
                    google }}</span>
            </button>
            <button
                class="w-300 h-38 md:w-300 md:h-38 rounded-30 mb-3 flex pb-1 items-center text-14 justify-center font-bold text-black bg-255 cursor-pointer hover:bg-230">
                <span class="f  mb-2 "> <img class="-ml-6 mt-3 -mb-5 " src="../assets/apple.svg" alt=""> {{ apple }}</span>
            </button>
            <button
                class="w-300 h-38 rounded-30 text-15 flex justify-center items-center  font-bold text-black bg-255 cursor-pointer hover:bg-230">
                <span class="font-twitter mt-2 mb-2 ">{{ account }}</span>
            </button>
        </div>
        <div class="text-148 text-13 pl-2 contrast-150">
            By signing up, you agree to the <span class="text-29  cursor-pointer hover:underline ">Terms of Service</span>
            and <span class="text-29 cursor-pointer hover:underline">Privacy Policy</span>, including <span
                class="text-29 cursor-pointer hover:underline">Cookie Use</span>.


        </div>
        <div
            class=" font-twitter flex  absolute top-80  text-#71767b left-8  text-13 font-normal -ml-5 contrast-150 cursor-pointer ">
            <p> <span class="hover:underline">Hizmet şartları</span> <span class=" ml-1 hover:underline ">Gizlilik
                    Politikası</span> <span class=" ml-1 hover:underline ">Çerez Politikası </span> <br>
                <span class=" -ml-0 mr-1 hover:underline">İmprint</span> <span
                    class="hover:underline">Erişebilirlik</span><span class=" ml-1 hover:underline"> Reklam Bilgisi</span>
                <br> <span class="hover:underline">DahaFazla...</span> &emsp;
                © 2023 Twitter, Inc
            </p>

        </div>



    </div>
</template>

<script>
export default {
    name: 'Makelogin',
    data() {
        return {
            user: "Kişiselleştirilmiş zaman akışını almak için hemen kaydol !",
            google: "Google ile Kaydolun",
            apple: "Apple ile Kaydol",
            account: "Hesap oluştur",
            twitterNew: "Twitter'da yeni misin?"
        }
    }
}
</script>

