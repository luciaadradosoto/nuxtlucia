<template>
    <div>
<img :src="product.image" alt=""srcset="">
<p> {{ product.title }}</p>
<NuxtLink :to="`/product/${product.id}`">
<p class="btn my-4 text-center"> Ver Detalle</p>
</NuxtLink>
    </div>
</template>

<script setup>

const { product } = defineProps(["product"])
</script>

<style scoped>
img{
    max-height:120px;
    max-width: 70%;
    margin:auto
}
</style>