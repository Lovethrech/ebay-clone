<script setup>
import TopNavDealCtn from "@/components/TopNavDealCtn.vue";
import TopNavPersonalsCtn from "@/components/TopNavPersonalsCtn.vue";
</script>

<style scoped>
.ctn{
    padding:0 7vw;
}
.main-ctn{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
}
i{
    color:rgb(0, 0, 0);
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
    background-color:rgb(255, 255, 255);
    padding:6px;
    border-radius:30px;
    font-size: 12px;
    border:2px dotted rgb(0, 0, 0);
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
/*
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
*/
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
                    <!-- <i class='bx bxs-moon' style='color:#efebeb' ></i> -->
                </div>
                
            </div>
            
        </div>
    </div>
</template>