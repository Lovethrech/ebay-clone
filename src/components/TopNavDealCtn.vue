<script setup>
import navDeals from "@/data/nav-deals.json";
</script>

<style scoped>
ul{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
    gap:20px;
}
li{
    color:hsl(0, 0%, 100%);
    text-transform:capitalize;
    font-size:12px;
}
li:hover{
    cursor:pointer;
    color:rgb(22, 202, 37);
    transition: all .6s;
}
</style>

<template>
    <ul>
        <li v-for="navDeal in navDeals" :key="navDeal.id">{{navDeal.name}}</li>
    </ul>
</template>