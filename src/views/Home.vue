<template>
  <div class="home">
    <NavBar />
    <FirstBanner  />
    <BannerHeader class="hidden sm:hidden md:block" Header="Partners" Desc="You prepare the food, we handle the rest" />
    <SecondBanner heading="List your restaurant or shop on foodpanda" pera1="Would you like millions of new customers to enjoy your amazing food and groceries? So would we!" pera2="It's simple: we list your menu and product lists online, help you process orders, pick them up, and deliver them to hungry pandas – in a heartbeat!" pera3="Interested? Let's start our partnership today!" bgImage="https://images.deliveryhero.io/image/foodpanda/home-vendor-pk.jpg?width=1400&height=896" />
     <BannerHeader class="hidden sm:hidden md:block" Header="Cities" Desc="Find us in these cities and many more!" />
     <Cities />
     <BannerHeader class="hidden sm:hidden md:block" Header="App" Desc="Put us in your pocket" />
      <AppDescBanner />
     <BannerHeader class="hidden sm:hidden md:block" Header="Office" Desc="Take your office out to lunch" />
     <SecondBanner heading="Foodpanda for business" pera1="Order lunch or fuel for work-from-home, late nights in the office, corporate events, client meetings, and much more." bgImage="https://images.deliveryhero.io/image/foodpanda/home-corporate-pk.jpg?width=1400&height=896" />
     <Footer />
    <!-- <div>
    <h1>Haider is live</h1>
    </div> -->
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/Header/Header.vue'
import FirstBanner from '../components/HomePageFirstBanner/HomePageFrstBanner.vue'
import BannerHeader from '../components/HeadingComponent/HeadingComponent.vue'
import SecondBanner from '../components/SecondBanner/SecondBanner.vue'
import Cities from '../components/Cities/Cities.vue'
import Footer from '../components/Footer/Footer.vue'
import AppDescBanner from '../components/AppHomeBanner/AppHomeBanner.vue'
export default {
  name: "Home",
  components: {
    NavBar,
    Footer,
    AppDescBanner,
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
