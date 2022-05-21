<template>
  <div class="main max-w-7xl mx-auto py-8 mb-5 flex justify-between items-center">
      <div class="textRight text-2xl font-medium ">
          foodpanda
      </div>
      <div class="signature">
          Muhammad Mudassir Siddiqui
      </div>
      <div class="leftSection flex justify-center items-center cursor-pointer">
          <div class="iconCover flex justify-center items-center">
              <i class="fa-brands fa-facebook-f"></i>
          </div>
          <div class="iconCover flex justify-center items-center mx-2">
              <i class="fa-brands fa-instagram"></i>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.signature{
    font-family: 'Water Brush', cursive;
    font-size: 60px;
}
.iconCover {
    width:40px;
    height: 40px;
    border: 1px solid lightgrey;
    border-radius: 50%;
}
.fa-brands {
    font-size:22px;
    color: grey;
}
.main {
    overflow: hidden;
    border-top: 1px solid lightgrey;
    border-bottom: 1px solid lightgrey;
}
.textRight {
    color: grey;
}
</style>