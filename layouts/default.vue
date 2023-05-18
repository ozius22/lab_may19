<template>
    <header>
        <nav>
            <NuxtLink to="/">Lab</NuxtLink>
            <ul>
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/Products/">Products</NuxtLink></li>
            </ul>
        </nav>
    </header>

    <div>
        <slot />
    </div>
</template>

<style>
    .router-link-exact-active {
        color: red;
    }
</style>