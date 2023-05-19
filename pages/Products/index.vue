<template>
    <div>
        <div class="grid grid-cols-3 gap-8">
            <div v-for="p in products">
            <NuxtLink :to="`/Products/${p.id}`">
            <img :src="p.image" alt="Product Image">
            {{ p.title }}
            </NuxtLink>
            </div>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'products'
    })

    const { data: products } = await useFetch('https://fakestoreapi.com/products')

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