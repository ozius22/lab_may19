<template>
    <div>
        <p>Product details for {{ id }}</p>
        <p>Few details about products. and then a few and the a few and then a few expounding ideas.</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params
</script>

<style scoped>

</style>
