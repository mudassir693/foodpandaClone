<template>
  <div class="home">
    <NavBar />
    <FirstBanner />
    <h1>Haider is live</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/Header/Header.vue'
import FirstBanner from '../components/HomePageFirstBanner/HomePageFrstBanner.vue'

export default {
  name: "Home",
  components: {
    NavBar,
    FirstBanner
  },
};
</script>
