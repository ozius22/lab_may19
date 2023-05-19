<template>
    <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between">
            <NuxtLink to="/" class="font-bold">Just Another Store</NuxtLink>
            <ul class="flex gap-4">
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/Products/" class="btn">Products</NuxtLink></li>
            </ul>
        </nav>
    </header>

    <div class="container mx-auto p-4">
        <slot />
    </div>
</template>

<style>
    .router-link-exact-active {
        color: red;
    }
</style>