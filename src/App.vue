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
      <nav class="nav_bar w-full h-[120px] bg-neutral-200 flex justify-between py-5 px-14">
        <img src="./assets/KAIA-LOGO-notext.png" alt="">
        <div class="flex items-center gap-12">
          <li>
            <a href="" class="py-3 text-4xl hover:text-amber-500">DESIGN</a>
          </li>
          <li >
            <a href="" class="py-3 text-4xl hover:text-amber-500">CODE</a>
          </li>
          <li >
            <a href="" class="py-3 text-4xl hover:text-amber-500">ABOUT</a>
          </li>
        </div>
      </nav>
    </header>
    <main class="flex flex-col w-screen items-center gap-36">
      <!-- banner -->
      <section class="w-full">
        <img src="./assets/orange-cloud.jpg" class="w-full" alt="">
      </section>
      <!-- design區段 -->
      <section class="flex flex-col w-full p-5">
        <div class="text-[200px] font-bold text-start text-stone-500">Design</div>
        <!-- <div class="w-[1700px] h-[2px] bg-stone-400 rotate-45 translate-y-[600px] "></div> -->
        <div class="flex flex-col gap-5 mb-5">
            <div class="text-4xl font-bold text-end pr-8 leading-snug">UI/UX設計│平面設計│3D建置</div>
            <div class="text-2xl text-end pr-8 leading-snug">設計不僅僅是美學的表達，更是溝通的藝術<br>每個設計作品都代表一段故事、一個品牌的靈魂、一種價值的傳遞</div>  
        </div>
        <!-- Swiper -->
        <swiper :slidesPerView="4" :spaceBetween="30" :centeredSlides="true" :pagination="{
            clickable: true,
          }" :modules="modules"
          class="mySwiper w-full h-[800px] flex">
          <swiper-slide class="swiper-slide hover:scale-105">
            <a href="">
              <img src="./assets/KAIASelectShop-1x1-2.png" alt="">
              <div class="slide-item">
                <span class="text-3xl font-bold">KAIA Select Shop<br>網站設計</span>
                <span class="text-2xl">為居家選物品牌創建線上購物平台，展現品牌的獨特風格和價值傳遞。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide hover:scale-105">
            <a href="">
              <img src="./assets/KAIASelectShop-1x1-2.png" alt="">
              <div class="slide-item">
                <span class="text-3xl font-bold">KAIA Select Shop<br>網站設計</span>
                <span class="text-2xl">為居家選物品牌創建線上購物平台，展現品牌的獨特風格和價值傳遞。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide hover:scale-105">
            <a href="">
              <img src="./assets/KAIASelectShop-1x1-2.png" alt="">
              <div class="slide-item">
                <span class="text-3xl font-bold">KAIA Select Shop<br>網站設計</span>
                <span class="text-2xl">為居家選物品牌創建線上購物平台，展現品牌的獨特風格和價值傳遞。</span>
              </div>  
            </a>
          </swiper-slide>
          <swiper-slide class="swiper-slide hover:scale-105">
            <a href="">
              <img src="./assets/KAIASelectShop-1x1-2.png" alt="">
              <div class="slide-item">
                <span class="text-3xl font-bold">KAIA Select Shop<br>網站設計</span>
                <span class="text-2xl">為居家選物品牌創建線上購物平台，展現品牌的獨特風格和價值傳遞。</span>
              </div>  
            </a>
          </swiper-slide>
        </swiper>
      </section>
      <section class="code-area flex w-full p-5 gap-6">
        <div class="w-11/12 flex flex-col gap-[100px] pl-[100px] py-[100px] ">
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-300 bg-opacity-40 hover:bg-opacity-60">
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/microsoft.png" alt="">
            <div class="w-5/12 flex flex-col justify-end gap-5 p-8">
              <span class="text-3xl font-bold">Microsoft 網站首頁</span>
              <span class="text-2xl">前端切版</span>
            </div>
          </a>
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-300 bg-opacity-40 hover:bg-opacity-60">
            <div class="w-5/12 flex flex-col justify-end gap-5 p-8">
              <span class="text-3xl font-bold">Microsoft 網站首頁</span>
              <span class="text-2xl">前端切版</span>
            </div>
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/microsoft.png" alt="">
          </a>
          <a href="" class="w-full h-[500px] flex flex-row rounded-3xl bg-stone-300 bg-opacity-40 hover:bg-opacity-60">
            <img class="w-7/12 object-cover object-top rounded-3xl shadow-xl z-10" src="./assets/microsoft.png" alt="">
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
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }
li{
  list-style: none;
}
.code-title{
  writing-mode: vertical-rl;
}
.code-area{
  background-image: url(./assets/white.jpg);
  background-size: cover;
}

.swiper-slide {
  width: 400px;
  height: 85%;
  text-align: center;
  font-size: 18px;
  background: #fff;
  /* Center slide text vertically */
  display: flex;
  flex-direction: column;
  margin:auto;
  border-radius: 20px;
  box-shadow: 0 0 10px 5px #c2c2c2;
}

.swiper-slide img {
  display: block;
  width: 100%;
  object-fit: cover;
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
