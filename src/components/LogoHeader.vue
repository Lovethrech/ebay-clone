<script setup>
import LogoCtn from "@/components/LogoCtn.vue";
import LogoShopTab from "@/components/LogoShopTab.vue";
import SearchTab from "@/components/SearchTab.vue";
</script>

<style scoped>
.ctn{
    padding: 1vh 7vw;
}
.main-ctn{
    display:flex;
    flex-direction:row;
    justify-content:space-between;
}
.logo-shop{
    display:flex;
    justify-content: space-between;
    gap:1px;
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
        </div>
    </div>
</template>