<style scoped>
.logo-ctn{
    width:80px;
    height:50px;
    background-color: black;
    padding:0 10px;
    display:flex;
    justify-content:center;
    place-items:center;
    border: 8px double rgb(255, 246, 246);
}
.logo-ctn:hover{
    cursor:pointer;
    transition:all .4s ease-in-out;
}
.logo-ctn img{
    width:100%;
    height:80%;
    margin:0 30px;
}
</style>

<template>
    <div class="logo-ctn">
        <img src="/Chel logo.svg" alt="Chel logo"/>
    </div>
</template>