<style scoped>
.ctn{
    padding: 0;
    width:100%;
    margin-left:30px;
}
.main-ctn, .desc{
    display:flex;
    flex-direction:row;
}
.main-ctn input{
    height:40px;
}
.search-icon{
    display:flex;
    justify-content: center;
    place-items: center;
}
.search-icon i{
    position:absolute;
    top:68px;
    left:21vw;
}
.main-ctn input{
    width:100%;
    background-color:transparent;
    padding:0 28px;
    border-radius:20px;
}
.all-cat{
    display:flex;
    justify-content:center;
    place-items: center;
    margin-left:-135px;
    border:0;
    border-left: 1px solid rgb(163, 158, 158);
    padding: 0 10px;
    border-radius:0 20px 20px 0;
}
.desc{
    margin:auto 0;
}
</style>

<template>
    <div class="ctn">
        <div class="main-ctn">
            <div class="search-icon">
                <i class='bx bx-search-alt-2'></i>
            </div>
            <input type="text" name="search" placeholder="Search for anything">
            <div class="all-cat">
                <div class="desc">
                    <p>All Categories</p>
                    <i class='bx bx-chevron-down'></i>
                </div>
            </div>
        </div>
    </div>
</template>