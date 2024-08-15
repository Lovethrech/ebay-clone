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
    flex-direction: row;
    justify-content: space-between;
}
</style>

<template>
    <div class="ctn">
        <div class="main-ctn">
            <RouterLink to="/">
                <LogoCtn></LogoCtn>
            </RouterLink>
            <LogoShopTab></LogoShopTab>
            <SearchTab></SearchTab>
        </div>
    </div>
</template>