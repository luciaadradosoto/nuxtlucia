<template>
   
       
    <div>
        <h1 class="text-3x1 font-bold mx-10 my-10 text bg-pink-400">
        </h1>
         <div class="grid grid-cols-4 gap-5 mx-10">   
        <div v-for="p in products"> 
       <ProductCard :product="p" />
    </div> 
    </div>
    </div>

    
</template> 
<script setup>
definePageMeta({
    layout: "products"
})

const { data: products } = await useFetch('https://fakestoreapi.com/products');
</script>

