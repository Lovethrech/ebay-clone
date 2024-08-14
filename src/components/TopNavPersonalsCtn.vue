<script setup>
import navPersonals from "@/data/nav-personals.json";
</script>

<style scoped>
ul{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
    gap:1vw;
}
li{
    color:hsl(0, 0%, 100%);
}
</style>

<template>
    <ul>
        <li v-for="navPersonal in navPersonals" :key="navPersonal.id">{{navPersonal.name}}</li>
    </ul>
</template>