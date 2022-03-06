<template>
    <div class="main mx-auto">
        <Header />
        <ResturantsTop class='my-10'/>
        <span class="text-3xl">
            Resturants
        </span>
    </div>
</template>
<script>
import Header from '../components/Header/Header.vue'
import ResturantsTop from '../components/ResturantsTop/ResturantsTop.vue'
export default {
    components:{
        Header,
        ResturantsTop
    }
}
</script>
<style scoped >
    
</style>