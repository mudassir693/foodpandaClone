<template>
  <div id="app">
    <!-- <input type="text" v-model="name"> -->
    <router-view />
  </div>
</template>
<script>

export default {
  data(){
    return {
      name:"Test",
      student:[]
    }
  },
  created(){
    this.$store.state.name="Changed"
    console.log(this.$store.state.name);
    this.sayHello()
  },
  methods:{
    sayHello(){
      console.log("object: ", this.name);
    }
  },
  watch:{
    name:function (val, lastValue) {
      this.sayHello()
      console.log('new value: ', val);
      console.log('last value: ', lastValue);
    },
  }
}
</script>


<style>


#app {
  font-family:  'Open Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
