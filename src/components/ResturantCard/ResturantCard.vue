<template>
    <div class="containerr cursor-pointer">
        <div class="imageContainer relative">
            <div class="imgWraper absolute top-0 left-0 ">
                <img class="image" src="https://images.deliveryhero.io/image/fd-pk/LH/s7rl-listing.jpg?width=400&height=292" alt="">
            </div>
            <div :class="true?'border-none':'border-white'"  class="loveContainer  border-2 flex justify-center rounded-full items-center absolute bottom-1 right-1">
                <i :class="true?'star':'text-white'" class="fa-solid fa-heart "></i>
            </div>
        </div>
        <div class="title flex justify-between mt-3 items-center">
            <div class="titleWrapper text-xl font-bold">
                Pizza Max
            </div>
            <div class="ratingWraper text-gray-500 text-sm">
                <i class="fa-solid mx-2 fa-star text-[#DA0060] star"></i>
                <span class="font-bold text-black">3.5</span>/5
            </div>
        </div>
        <div class="category text-gray-500  font-thin">
            $$$, pakistani
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.containerr{
    /* width: fit-content; */
     width: 100%;
    height: fit-content;
    /* background-color:red */
}
.imageContainer {
    width: 100%;
    height: 13rem;
    overflow:hidden;
    
}
.imgWraper {
    width: 100%;
    height: 100%;
    transition: all 200ms ease-in-out;
}
.image {
    object-fit:contain;
}
.containerr:hover .imgWraper {
    transform:scale(1.05)
}
.star {
    color: #DA0060;
}
.loveContainer {
    width: 28px;
    height: 28px;
}

</style>