<template>
<div class="main">

  <Header />
  <div class="mainContainer my-10">
  <div class="wrapperContainer grid grid-cols-3 gap-4 my-10 max-w-7xl bg-red-500 mx-auto">
    <div class="col-span-2">
        rightCloumn
    </div>
    <div class="col-span-1">
        left
    </div>
  </div>
  </div>
</div>
</template>

<script>
import Header from '../components/Header/Header.vue'
export default {
    components:{
        Header
    }
}
</script>

<style scoped>
    .wrapperContainer {
        height: 50px;
    }
</style>