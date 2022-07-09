<template>
    <div class="main">
        <div class="container max-w-7xl mx-auto my-2">
            <div class="allResturantsHeader text-3xl my-4 font-thin">
                All Resturants
            </div>
            <div class="allResturantsCards grid grid-cols-4 gap-4">
                <ResturantCard />
                <ResturantCard />
                <ResturantCard />
                <ResturantCard />
                <ResturantCard />
                <ResturantCard />
            </div>
        </div>
    </div>
</template>

<script>
import ResturantCard from '../ResturantCard/ResturantCard.vue'
export default {
    components:{
        ResturantCard
    }

}
</script>

<style scoped>
.container {
    overflow: hidden;
}

</style>