<script setup>
    import productsJSON from '@/assets/productos.json'
    function getProduct(id){
        return productsJSON.find((product) => product.id === id)
    };

</script>

<template>
    <li v-for="product in productsJSON" :key="product.id">
        <RouterLink :to="`/products/${product.id}`">{{ product.name }}</RouterLink>
    </li>
</template>
