<script setup>
    import ProductDetail from '@/components/ProductDetail.vue';
    import { useRoute } from 'vue-router';
    import productosJSON from '@/assets/productos.json'
    
    function getProduct(id){
        return productosJSON.find((product) => product.id === id);
    } 

    const route = useRoute();

    const product = getProduct(route.params.id);
    const { name, description, id } = product;
</script>

<template>
    <h2>Product detail</h2>
    <ProductDetail :name="name" :description="description" :id="id"></ProductDetail>
</template>