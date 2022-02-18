<template>
  <div class="home">
    <NavBar />
    <FirstBanner />
    <BannerHeader />
    <h1>Haider is live</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/Header/Header.vue'
import FirstBanner from '../components/HomePageFirstBanner/HomePageFrstBanner.vue'
import BannerHeader from '../components/HeadingComponent/HeadingComponent.vue'


export default {
  name: "Home",
  components: {
    NavBar,
    FirstBanner,
    BannerHeader
  },
};
</script>

<style scoped>
.home{
  /* overflow-x: hidden; */
}
</style>
