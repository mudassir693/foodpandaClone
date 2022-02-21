<template>
  <div class="home">
    <NavBar />
    <FirstBanner  />
    <BannerHeader Header="Partners" Desc="You prepare the food, we handle the rest" />
    <SecondBanner />
     <BannerHeader Header="Cities" Desc="Find us in these cities and many more!" />
    <div>
    <h1>Haider is live</h1>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/Header/Header.vue'
import FirstBanner from '../components/HomePageFirstBanner/HomePageFrstBanner.vue'
import BannerHeader from '../components/HeadingComponent/HeadingComponent.vue'
import SecondBanner from '../components/SecondBanner/SecondBanner.vue'

export default {
  name: "Home",
  components: {
    NavBar,
    FirstBanner,
    BannerHeader,
    SecondBanner
  },
};
</script>

<style scoped>
.home{
  /* overflow-x: hidden; */
}
</style>
