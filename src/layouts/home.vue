<template>
  <main class="px-4 py-10 text-center text-gray-700 dark:text-gray-200">
    <router-view />
    <Footer />
    <div class="mt-5 mx-auto text-center opacity-25 text-sm">
      [Home Layout]
    </div>
  </main>
</template>
<style scoped>
main::before{
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
  opacity: 0.11;
}
</style>
