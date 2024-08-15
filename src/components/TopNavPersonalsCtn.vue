<script setup>
import navPersonals from "@/data/nav-personals.json";
</script>

<style scoped>
ul{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
    gap:20px;
}
li{
    display: flex;
    flex-direction:row;
    justify-content:center;
    place-items:center;
    color:hsl(0, 0%, 0%);
    font-size:10px;
}
li:hover{
    cursor:pointer;
    color:rgb(22, 202, 37);
    transition: all .6s;
}

@media screen and (max-width:970px) {
    li:nth-child(2){
        display:none;
    }
}
@media screen and (max-width:550px) {
    li:nth-child(1) {
        display: none;
    }
}
</style>

<template>
    <ul>
        <li 
            v-for="navPersonal in navPersonals" 
            :key="navPersonal.id"
        >
                {{navPersonal.name}}
                <div class="icons" v-html="navPersonal.icon"></div>
        </li>
    </ul>
</template>