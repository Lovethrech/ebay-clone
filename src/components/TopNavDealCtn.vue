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
    color:hsl(0, 0%, 0%);
    text-transform:capitalize;
    font-size:10px;
}
li:hover{
    cursor:pointer;
    color:rgb(22, 202, 37);
    transition: all .6s;
}
@media screen and (max-width:750px) {
    li:nth-child(1), li:nth-child(2), li:nth-child(4){
        display: none;
    }
}
</style>

<template>
    <ul>
        <li v-for="navDeal in navDeals" :key="navDeal.id">{{navDeal.name}}</li>
    </ul>
</template>