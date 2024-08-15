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
.user-icon, .personal-ctn{
    display:flex;
    flex-direction:row;
    justify-content: space-between;
    justify-content:center;
    place-items:center;
    gap:40px;
}
.user-icon i{
    background-color:rgb(23, 27, 23);
    padding:10px;
    border-radius:40px;
    font-size: 14px;
    border:2px dashed white;
}
.user-icon i:hover{
    cursor:pointer;
    transform: scale(0.94);
}
.notify-cart{
    display:flex;
    flex-direction: row;
    justify-content: space-between;
    gap:1vw;
}

.notify-cart i{
    display:flex;
    justify-content:center;
    place-items:center;
}
.notify-cart i:hover{
    cursor:pointer;
    color:rgb(22, 202, 37);
    transform:scale(1.2);
    transition: all .4s;
}
.notify-cart i:last-child{
    padding: 6px 20px;
    background-color:rgb(22, 85, 27);
    border-radius:20px;
    box-shadow: 0px 0px 8px 2px rgba(22, 85, 27, 0.719);
    font-size:10px;
}
.notify-cart i:last-child:hover{
    cursor:pointer;
    background-color:rgb(29, 121, 36);
    transform:scaleX(1.1);
    transition: all .4s;
}
@media screen and (max-width:550px) {
    .notify-cart i:nth-child(1) {
        display: none;
    }
    .personal-ctn{
        gap:20px;
    }
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
                    <i class='bx bx-bell' ></i>
                    <i class='bx bx-cart' ></i>
                    <!-- <i class='bx bx-moon' ></i> -->
                    <i class='bx bxs-moon' style='color:#efebeb' ></i>
                </div>
                
            </div>
            
        </div>
    </div>
</template>