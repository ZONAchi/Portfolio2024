<script setup>
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
</style>
