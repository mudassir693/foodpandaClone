<template>
  <div class="main py-3 px-2 mx-auto md:mx-0 flex justify-between items-cener rounded-lg cursor-pointer">
    <div class="right flex justify-between items-cener flex-col">
        <div class="topContainer">
            <div class="name text-xl">Chicken Patties</div>
            <div class="name text-gray-400">Serve 2 person</div>
        </div>
        <div class="price text-lg font-thin">Rs: 500</div>
    </div>
    <div class="image bg-white">
        <div class="imgContainer rounded overflow-hidden relative">
            <img class="img" src="https://images.deliveryhero.io/image/fd-pk/LH/s7rl-listing.jpg?width=400&height=292" alt="">
            <div class="plusContainer absolute bottom-0 right-0 z-99 flex justify-center items-center rounded">
                <i class="fa-solid fa-plus text-white"></i>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main {
    width: 98%;
    /* background: #DA0060; */
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    /* height: 105px; */
    height: 130px;
}
.imgContainer {
    width: 7rem;
    height: 100%;
    object-fit:cover;
}
.img {
    height: 100%;
    object-fit:cover;
}
.plusContainer {
    width: 2rem;
    height: 2rem;
    background-color:#DA0060;
}
</style>