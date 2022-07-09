<template>
    <div class="main mx-auto">
        <Header />
        <ResturantsTop class='my-10'/>
        <AllResturants />
        <span class="text-3xl">
            Resturants
        </span>
    </div>
</template>
<script>
import Header from '../components/Header/Header.vue'
import ResturantsTop from '../components/ResturantsTop/ResturantsTop.vue'
import AllResturants from '../components/AllResturants/AllResturants.vue'
export default {
    components:{
        Header,
        AllResturants,
        ResturantsTop
    }
}
</script>
<style scoped >
    .main {
        overflow: hidden;
    }
</style>