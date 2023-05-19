<template>
    <div class="container px-4 mx-auto justify-center">
        <img :src="product.image" alt="Product Image">
        <p class="font-bold mt-4">{{ product.title }}</p>
        <p>{{ product.price }}</p>
        <p>{{ product.description }}</p>
        <p>{{ product.rating }}</p>
        <p>{{ product.reviews }}</p>
        
    </div>
</template>

<script setup>
    const { id } = useRoute().params

    const { data:product } = await useFetch('https://fakestoreapi.com/products/' + id)

    definePageMeta({
        layout: 'products'
    })
</script>

<style scoped>

</style>
