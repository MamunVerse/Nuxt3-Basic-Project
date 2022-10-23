<template>
    <h1>Iphone 14 {{ name }}</h1>
</template>

<script setup>

    const route = useRoute();

    const name = computed(()=>{
        return route.params.name.replaceAll('-', ' ');
    })
</script>