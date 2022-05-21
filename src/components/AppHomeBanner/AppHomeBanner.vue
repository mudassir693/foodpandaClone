<template>
  <div class="main bg-[#E21B70] relative py-10">
      <div class="px-5 md:px-0  max-w-7xl relative mx-auto text-2xl text-white my-10">
          <div class="containerDiv">
            <div class="textContainerHeader text-3xl font-thin">
                Download the food and groceries you love
            </div>
            <div class="textContainerHeader text-xl my-5 font-thin max-w-3xl">
                It's all at your fingertips – the restaurants and shops you love. Find the right food and groceries to suit your mood, and make the first bite last. Go ahead, download us.
            </div>
          </div>

          <div class= "imageContainer hidden sm:hidden md:block">
            <img class="image" src="../../assets/home-foodpanda-apps.webp" alt="">
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.main {
    background-color: #E21B70;
    opacity: 0.9
}
.imageContainer {
    position: absolute;
    /* right: 0px; */
    top: -150%;
    right: -10%;
}
.image {
    height:500px;
    object-fit:contain;
}
</style>