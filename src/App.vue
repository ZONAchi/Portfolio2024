<script>
import { register } from 'swiper/element/bundle';
register();
 // Import Swiper Vue.js components
 import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';


// import required modules
import { Pagination } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>

<template>
  <header>
      <nav class="w-full nav_bar h-24 lg:h-28 py-5 lg:px-14 bg-neutral-50 md:bg-neutral-50/75 flex flex-col gap-4 md:flex-row justify-between items-center fixed top-0 z-20">
        <img class="h-8 px-8 lg:h-16 object-contain" src="./assets/KAIA-LOGO-notext.png" alt="">
        <div class="flex w-full md:w-auto px-8 items-center justify-between gap-8 md:gap-12 bg-neutral-300 md:bg-transparent">
          <li>
            <a href="" class="py-3 text-lg md:text-2xl lg:text-4xl hover:text-amber-500">DESIGN</a>
          </li>
          <li >
            <a href="" class="py-3 text-lg md:text-2xl lg:text-4xl hover:text-amber-500">CODE</a>
          </li>
          <li >
            <a href="" class="py-3 text-lg md:text-2xl lg:text-4xl hover:text-amber-500">ABOUT</a>
          </li>
        </div>
      </nav>
      <!-- banner -->
      <section class="w-full">
        <img src="./assets/orange-cloud.jpg" class="w-full h-72 md:h-96 lg:h-screen object-cover" alt="">
      </section>
    </header>
    <main class="w-full flex flex-col items-center gap-8">
      <!-- design區段 -->
      <section class="flex flex-col w-full">
        <div class="ml-[50px] lg-ml-[100px]">
          <div class="text-5xl md:text-[80px] lg:text-[200px] font-bold text-start text-stone-500">Design . . . </div>
          <!-- <div class="w-[1700px] h-[2px] bg-stone-400 rotate-45 translate-y-[600px] "></div> -->
          <div class="flex flex-col gap-5 mb-5 px-4">
              <div class="text-xl lg:text-4xl font-bold pr-8 leading-snug">UI/UX設計│平面設計│3D建置</div>
              <div class="text-base lg:text-2xl pr-8 leading-snug">設計是美學的表達，更是溝通的藝術<br>每個設計作品都代表一段故事、一個品牌的靈魂、一種價值的傳遞</div>  
          </div>
        </div>
        
        <!-- Swiper -->
        <swiper :slidesPerView="1" :breakpoints="{768: {slidesPerView: 2 , centeredSlides:false}, 1280: {slidesPerView: 4 ,centeredSlides:true}}" :spaceBetween="30" :modules="modules"
          class="mySwiper w-full h:[600px] lg:h-[700px] flex">
          <swiper-slide class="swiper-slide">
            <a href="">
              <img class="h-[300px]" src="./assets/KAIASelectShop-4x3.png" alt="">
              <div class="slide-item">
                <span class="text-lg lg:text-2xl font-bold">KAIA Select Shop<br>品牌網站設計</span>
                <span class="text-base lg:text-xl text-ellipsis">為使用者提供清新、舒適的線上購物平台，呈現品質家居用品和生活美學。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <a href="">
              <img class="h-[300px]" src="./assets/KAIASelectShop-4x3.png" alt="">
              <div class="slide-item">
                <span class="text-xl lg:text-2xl font-bold">KAIA Select Shop<br>品牌網站設計</span>
                <span class="text-base lg:text-xl text-ellipsis">為使用者提供清新、舒適的線上購物平台，呈現品質家居用品和生活美學。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <a href="">
              <img class="h-[300px]" src="./assets/KAIASelectShop-4x3.png" alt="">
              <div class="slide-item">
                <span class="text-xl lg:text-2xl font-bold">KAIA Select Shop<br>品牌網站設計</span>
                <span class="text-base lg:text-xl text-ellipsis">為使用者提供清新、舒適的線上購物平台，呈現品質家居用品和生活美學。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <a href="">
              <img class="h-[300px]" src="./assets/KAIASelectShop-4x3.png" alt="">
              <div class="slide-item">
                <span class="text-xl lg:text-2xl font-bold">KAIA Select Shop<br>品牌網站設計</span>
                <span class="text-base lg:text-xl text-ellipsis">為使用者提供清新、舒適的線上購物平台，呈現品質家居用品和生活美學。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide">
            <a href="">
              <img class="h-[300px]" src="./assets/KAIASelectShop-4x3.png" alt="">
              <div class="slide-item">
                <span class="text-xl lg:text-2xl font-bold">KAIA Select Shop<br>品牌網站設計</span>
                <span class="text-base lg:text-xl text-ellipsis">為使用者提供清新、舒適的線上購物平台，呈現品質家居用品和生活美學。</span>
              </div>  
            </a>
          </swiper-slide>
        </swiper>
      </section>
      <section class="code-area flex w-full p-5 gap-6">
        <div class="w-11/12 flex flex-col gap-[100px] pl-[100px] py-[100px] ">
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-50 bg-opacity-40 hover:bg-stone-50 hover:bg-opacity-80">
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/microsoft.png" alt="">
            <div class="w-5/12 flex flex-col justify-end gap-5 p-8">
              <span class="text-3xl font-bold">Microsoft 網站首頁</span>
              <span class="text-2xl">前端切版</span>
            </div>
          </a>
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-50 bg-opacity-40 hover:bg-stone-50 hover:bg-opacity-80">
            <div class="w-5/12 flex flex-col justify-end gap-5 p-8">
              <span class="text-3xl font-bold">Microsoft 網站首頁</span>
              <span class="text-2xl">前端切版</span>
            </div>
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/COFFEE1920x1080.png" alt="">
          </a>
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-50 bg-opacity-40 hover:bg-stone-50 hover:bg-opacity-80">
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/Frame 37.png" alt="">
            <div class="w-5/12 flex flex-col justify-end gap-5 p-8">
              <span class="text-3xl font-bold">Microsoft 網站首頁</span>
              <span class="text-2xl">前端切版</span>
            </div>
          </a>
        </div>
        <div class="code-title text-[200px] font-bold -translate-y-28 text-stone-500">Code . . . . . . . . . </div>
      </section>
      <section class="flex flex-col w-full p-8 gap-6 mb-[100px]">
        <div class="text-[200px] font-bold translate-y-44 text-stone-500">About</div>
        <div class="w-full h-[700px] flex p-8">
          <img class="w-1/2 h-full" src="./assets/bg-blueorange.jpg" alt="">
          <div class="w-1/2 h-full p-8 flex flex-col justify-end">
            <span class="text-4xl">title</span>
            <span>text</span>
          </div>
        </div>
        <button>more</button>
      </section>
    </main>
    <footer>
      <div class="flex w-full h-[300px] p-8 gap-6 bg-stone-300"></div>
    </footer>
  <RouterView />
</template>

<style scoped>
* {
    box-sizing: border-box;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    line-height: 1.5;
  }
li{
  list-style: none;
}

.code-title{
  writing-mode: vertical-rl;
}
.code-area{
  background-image: url(./assets/bg-blueorange.jpg);
  background-size: cover;
}

.mySwiper{
  padding: 8px;
}

.swiper-slide {
  height: 80%;
  text-align: center;
  font-size: 18px;
  background: #fff;
  /* Center slide text vertically */
  display: flex;
  flex-direction: column;
  border-radius: 20px;
  box-shadow: 0 0 10px 2px #e1e1e1;
}

.swiper-slide img {
  display: block;
  width: 100%;
  object-fit: cover;
  object-position: top;
  border-radius: 20px;
}

.slide-item{
  width: 100%;
  padding: 24px;
  text-align: start;
  display: flex;
  flex-direction: column;
  gap: 12px;
}
</style>
