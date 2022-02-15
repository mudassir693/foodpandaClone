<template>
  <div class="home">
    <NavBar />
    <h1>Haider is live</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '../components/Header/Header.vue'

export default {
  name: "Home",
  components: {
    NavBar
  },
};
</script>
