<template>
    <div>
        <ProductDetail :product ="product"/>
    </div>       
</template>
<script setup>
//paginas productos 

    const { id } = useRoute().params
</script>