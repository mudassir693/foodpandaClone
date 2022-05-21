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
  /* overflow-x: hidden; */
  margin:0;
  overflow-x:hidden;
  padding: 0;box-sizing: border-box;
}
</style>
