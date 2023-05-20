<template>
    <div class="bg-green-900 p-10 rounded-lg">
        <div class="grid grid-cols-3 gap-4">
            <div v-for="p in products" class="bg-white rounded-lg p-20">
                <NuxtLink :to="`/Products/${p.id}`">
                    <div class="aspect-w-2 aspect-h-1">
                        <img :src="p.image" alt="Product Image" class="object-cover rounded-lg">
                    </div>
                    <p class="text-black font-semibold mt-4 text-center">{{ p.title }}</p>
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