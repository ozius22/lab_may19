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

    <section>
        <h2>Home</h2>
        <p>Text goes here.</p>
        <p>And, also here.</p>
        <p>As well as here.</p>
    </section>
</template>

<script setup>

</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }

    p {
        margin: 20px 0;
    }
</style>