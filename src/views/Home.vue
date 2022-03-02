<template>
  <div class="home">
    <NavBar />
    <FirstBanner  />
    <BannerHeader class="hidden sm:hidden md:block" Header="Partners" Desc="You prepare the food, we handle the rest" />
    <SecondBanner heading="List your restaurant or shop on foodpanda" bgImage="https://images.deliveryhero.io/image/foodpanda/home-vendor-pk.jpg?width=1400&height=896" />
     <BannerHeader class="hidden sm:hidden md:block" Header="Cities" Desc="Find us in these cities and many more!" />
     <Cities />
     <BannerHeader class="hidden sm:hidden md:block" Header="Office" Desc="Take your office out to lunch" />
     <SecondBanner heading="Foodpanda for business" bgImage="https://images.deliveryhero.io/image/foodpanda/home-corporate-pk.jpg?width=1400&height=896" />
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
import Cities from '../components/Cities/Cities.vue'

export default {
  name: "Home",
  components: {
    NavBar,
    FirstBanner,
    BannerHeader,
    SecondBanner,
    Cities
  },
};
</script>

<style scoped>
.home{
  /* overflow-x: hidden; */
}
</style>
