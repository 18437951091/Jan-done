<template>
  <main class="text-center text-gray-700 dark:text-gray-200">
    <div id="head" class="w-full relative border-b-1 border-gray-200 bg-gray-100 dark:(border-gray-700 bg-gray-800) shadow-md sticky top-0 z-1">
      <nav id="navbar" ref="el" class="h-12 transform m-auto container flex justify-between">
        <div class="self-center animate-heart-beat animate-count-infinity">
          <a href="/">
            <img id="logo" src="/favicon.svg" alt="" class="inline h-12">
            <span>Jan Done</span>
          </a>
        </div>
        <Footer />
      </nav>
    </div>
    <div id="content" class="container pt-5 m-auto">
      <router-view />
    </div>
    <div class="mt-5 mx-auto opacity-25 text-sm">
      [Default Layout]
    </div>
  </main>
</template>
<script setup lang="ts">

</script>

<style>
#head::before{
  z-index: -1;
  content: '';
  position:absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  background-image: url(/images/fish.svg);
  background-repeat: repeat;
  background-position:center;
  opacity: 66%;
}
#content::before{
  z-index: -2;
  content: '';
  position:fixed;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  background-image: url(/images/triangle.svg);
  background-size: 75%;
  background-repeat: repeat;
  opacity: 0.1;
}
</style>
