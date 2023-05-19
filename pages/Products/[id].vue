<template>
    <div>
        <p>{{ product.title }}</p>
        <p>{{ product.price }}</p>
        <p>{{ product.id }}</p>
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
