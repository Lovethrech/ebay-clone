<style scoped>
.ctn{

}
.main-ctn, .desc{
    display:flex;
    flex-direction:row;
}
.main-ctn input{
    width:40vw;
    height:30px;
}
.search-icon{
    display:flex;
    justify-content: center;
    place-items: center;
}
</style>

<template>
    <div class="ctn">
        <div class="main-ctn">
            <div class="search-icon">
                <i class='bx bx-search-alt-2'></i>
            </div>
            <input type="text" name="search">
            <div class="all-cat">
                <div class="desc">
                    <p>All <br> Categories</p>
                    <i class='bx bx-chevron-down'></i>
                </div>
            </div>
        </div>
    </div>
</template>