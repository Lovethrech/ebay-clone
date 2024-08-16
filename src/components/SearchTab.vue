<style scoped>
.ctn{

}
.main-ctn, .desc{
    display:flex;
    flex-direction:row;
}
.main-ctn input{
    width:40vw;
    height:40px;
}
.search-icon{
    display:flex;
    justify-content: center;
    place-items: center;
    margin-right:-20px;
}
.main-ctn input{
    background-color:transparent;
    padding:0 20px;
    border-radius:20px;
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