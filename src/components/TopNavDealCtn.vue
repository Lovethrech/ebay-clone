<script setup>
import navDeals from "@/data/nav-deals.json";
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
    text-transform:capitalize;
}
</style>

<template>
    <ul>
        <li v-for="navDeal in navDeals" :key="navDeal.id">{{navDeal.name}}</li>
    </ul>
</template>