<template>
<div class="main">

  <Header />
  <div class="mainContainer my-10">
  <div class="wrapperContainer relative grid grid-cols-4 my-10 max-w-7xl mx-auto">
    <div class="col-span-4 md:col-span-3 ">
        <ResturantProfleConponent />
    </div>
    <div class="col-span-1 hidden md:block ">
        <CartComponent />
    </div>
  </div>
  </div>
  <Footer />
</div>
</template>

<script>
import Header from '../components/Header/Header.vue'
import ResturantProfleConponent from '../components/ResturantProfleConponent/ResturantProfleConponent.vue'
import CartComponent from '../components/CartComponent/CartComponent.vue'
import Footer from '../components/Footer/Footer.vue'
export default {
    components:{
    Header,
    ResturantProfleConponent,
    CartComponent,
    Footer
}
}
</script>

<style scoped>

</style>