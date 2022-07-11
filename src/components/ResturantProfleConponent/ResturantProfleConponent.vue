<template>
  <div class="mainn">
    <div class="wrapperr">
        <div class="imgContainer">
            <img class="img" src="https://images.deliveryhero.io/image/fd-pk/LH/s7rl-listing.jpg" alt="">
        </div>
        <div class="descriptionContainer my-3 px-3">
            <div class=" text-2xl font-bold">
                Pizza Max
            </div>
             <div class="ratingWraper text-gray-500 text-sm">
                <i class="fa-solid fa-star text-[#DA0060] star"></i>
                <span class="font-bold text-black star">3.5</span>/5
            </div>
            <div class="font-light text-gray-500 text-lg my-3">
                $$$, Pizza, Pakistani
            </div>
            <div class="address text-gray-500 text-lg font-light">
                B-70, Block H North Nazimabad Town, Karachi, Karachi City, Sindh
            </div>
        </div>
        <div class="py-5 dealsSection bg-gray-100 px-3">
            <div class="eachDeal my-2">
                <div class="text-black text-2xl font-bold">
                    EID DEAL - 10% OFF
                </div>
                <div class="dealDescription text-gray-500 text-base">
                    Enjoy 10% discount on entire menu |MOV=299| "Get additional 5% off being a pandapro member"
                </div>
            </div>
        </div>
        <div class="ResturantItems py-5">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <ResturantItemCard />
                <ResturantItemCard />

                <ResturantItemCard />
                <ResturantItemCard />

                <ResturantItemCard />
                <ResturantItemCard />

                <ResturantItemCard />
                <ResturantItemCard />
            </div>
        </div>
    </div>
    
  </div>
</template>

<script>
import ResturantItemCard from '../ResturantItemCard/ResturantItemCard.vue';
export default {
    components: { ResturantItemCard }
}
</script>

<style scoped>
/* .mainn {

} */
.img{
    object-fit:cover
}
.imgContainer {
    height:25rem;
    overflow: hidden;
    object-fit:cover;
    /* background:red; */
}
.star {
    color: #DA0060;
}

</style>