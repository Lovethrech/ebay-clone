<style scoped>
.ctn{
    color:black;
}
.desc{
    display:flex;
    flex-direction: row;

}
.dropdown-icon{
    display:flex;
    justify-content: center;
    place-items: center;
}
.desc p{
    font-size: 14px;
}
.dropdown-icon {
    font-size: 26px;
}
</style>

<template>
    <div class="ctn">
        <div class="desc">
            <p>Shop by <br>category</p>
            <div class="dropdown-icon">
                <i class='bx bx-chevron-down'></i>
            </div>
        </div>
    </div>
</template>