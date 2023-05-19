<template>
  <header class="shadow-sm bg-white text-[35px]">
    <nav class="container mx-auto p-4">
        <NuxtLink to="/Products" class="font-bold">Just Another Store Merch</NuxtLink>
    </nav>
  </header>

  <div class="container mx-auto p-4">
    <slot />
  </div>

  <footer class="container mx-auto p-4 flex justify-between border-t-2 font-bold">
    <ul class="flex gap-2">
      <li><NuxtLink to="/">Home</NuxtLink></li>
      <li><NuxtLink to="/Products/">Products</NuxtLink></li>
      </ul>
  </footer>
</template>

<style>
  .router-link-exact-active {
      color: green;
  }
</style>