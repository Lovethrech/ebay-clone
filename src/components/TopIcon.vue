<script setup>
import TopNavDealCtn from "@/components/TopNavDealCtn.vue";
import TopNavPersonalsCtn from "@/components/TopNavPersonalsCtn.vue";
</script>

<style scoped>
.ctn{
    padding:0 4vw;
}
.main-ctn{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
}
i{
    color:white;
}
.user-icon{
    display:flex;
    flex-direction:row;
    justify-content: space-between;
    gap:3vw;
}
</style>


<template>
    <div class="ctn">
        <div class="main-ctn">
            <div class="user-icon">
                <i class='bx bx-user'></i>
                <div class="deals-ctn">
                    <TopNavDealCtn></TopNavDealCtn>
                </div>
            </div>
            
            <div class="personal-ctn">
                <TopNavPersonalsCtn></TopNavPersonalsCtn>
                <div class="notify-cart">

                </div>
                
            </div>
            
        </div>
    </div>
</template>