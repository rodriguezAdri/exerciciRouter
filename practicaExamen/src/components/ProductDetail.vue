<script setup>
const { name, description, id } = defineProps({
    name: String,
    description: String,
    id: String
});
</script>

<template>
    <h2>{{ id }}</h2>
    <p>Nombre: {{ name }}</p>
    <p>Descripción: {{ description }}</p>
</template>