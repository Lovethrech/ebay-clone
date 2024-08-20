<script setup>
import LogoCtn from "@/components/LogoCtn.vue";
import LogoShopTab from "@/components/LogoShopTab.vue";
import SearchTab from "@/components/SearchTab.vue";
import SearchBtn from "@/components/SearchBtn.vue";
</script>

<style scoped>
.ctn{
    padding: 1vh 7vw;
}
.main-ctn{
    display:flex;
    flex-direction:row;
}
.logo-shop{
    display:flex;
    width:50px;
}
.main-ctn p{
    display:flex;
    justify-content: center;
    place-items: center;
    font-size:10px;
}
</style>

<template>
    <div class="ctn">
        <div class="main-ctn">
            <div class="logo-shop">
                <RouterLink to="/">
                    <LogoCtn></LogoCtn>
                </RouterLink>
                <LogoShopTab></LogoShopTab>    
            </div>            
            <SearchTab></SearchTab>
            <SearchBtn></SearchBtn>
            <p>Advanced Search</p>
        </div>
    </div>
</template>