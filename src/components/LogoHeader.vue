<script setup>
import LogoCtn from "@/components/LogoCtn.vue";
import LogoShopTab from "@/components/LogoShopTab.vue";
</script>

<style scoped>
.ctn{
    padding: 1vh 7vw;
}
.main-ctn{
    display:flex;
    flex-direction: row;
    justify-content: space-between;
    gap:10px;
}
</style>

<template>
    <div class="ctn">
        <div class="main-ctn">
            <RouterLink to="/">
                <LogoCtn></LogoCtn>
            </RouterLink>
            <LogoShopTab></LogoShopTab>
        </div>
    </div>
</template>