<template>
    <div style="" class="main">
        <div style="" class="container max-w-7xl mx-auto text-left">
            <div class="textSection flex  items-center flex-column  ">
                <div>
                <div class=" text text-5xl font-thin">
                    It's the food and groceries you love, delivered
                </div>
                <div class="inputBox my-5">
                    <div class="border border-grey-500 p-5 grid">
                        <div style="" class="inputContainer border border-grey-500 grid-cols-7 ">
                            <input class=" p-4" value="Haider" type="text">
                        </div>
                        <div class="or grid-cols-1">
                            Or
                        </div>
                        <div class="btn border border-grey-500 grid-cols-2 ">
                            Hello
                        </div>
                        <div class="btn border border-grey-500 grid-cols-2">
                            Hello
                        </div>
                    </div>
                </div>
                </div>
            </div>
        </div>
        <img class="banner" src="../../assets/hero-home-pk.webp" alt="">
    </div>
</template>


<script>

export default ({
    
})
</script>


<style scoped>
.main{
    height: 80vh;
    position: relative;
    z-index: 1;
    overflow-x: hidden;
}
.text {
    width: 80%;
    /* font-weight: 100;
    font-size: 3rem; */
    line-height:3.5rem;
}
.border {
    width: 80%;
}
.container ,.textSection {
    height: 100%;
}
.container {
    z-index: 8888;
}
.banner {
    /* width: ; */
    height: 100%;
    object-fit: contain;
    position:absolute;
    top: 0%;
    /* z-index: 100; */
    right: -30%;
}

</style>