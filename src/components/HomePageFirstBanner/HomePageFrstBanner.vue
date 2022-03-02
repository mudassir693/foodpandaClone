<template>
    <div style="" class="main  ">
        <div style="position:relative;" class="container max-w-7xl mx-auto text-left">
            <div  class="textSection flex items-center flex-column  ">
                <div  class="containerWrapper">
                <div class=" text text-5xl font-thin">
                    It's the food and groceries you love, delivered
                </div>
                <div class="inputBox my-5 ">
                    <div class="textContainer  border border-grey-500 p-5 flex">
                        <div  class="inputContainer cursor-pointer border border-grey-500  ">
                            <label for="inputFeild">
                            <input id="inputFeild" class="inputFeildContainer text-1xl p-4" placeholder="Enter your full address" type="text">
                            <span class="md:mx-2 lg:mx-2 cursor-pointer "><i class="navigatorIcon text-2xl fa-solid fa-location-crosshairs"></i></span>
                            </label>
                        </div>
                        
                        <div style="" class="btn text-1xl border border-grey-500 flex justify-center items-center mx-3 cursor-pointer">
                            Delivery
                        </div>
                        <div class="or flex justify-center items-center">
                            Or
                        </div>
                        <div style="" class="btn text-1xl border border-grey-500 flex justify-center items-center mx-3 cursor-pointer">
                            Pick-Up
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
.inputFeildContainer {
    width: 90%;
    border: none;
    outline: none;
}

.main{
    height: 80vh;
    position: relative;
    z-index: 1;
    overflow-x: hidden;
    max-height: 1000px;

    /* background:lightgray; */
}
.textContainer {
    border-radius: 0.5rem;
    box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
}
.containerWrapper{
    width: 75%;
}
.text {
    width: 100%;
    z-index: 9999;
    /* font-weight: 100;
    font-size: 3rem; */
    line-height:3.5rem;
}
.border {
    width: 100%;
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
    z-index: 1!important;
    max-height: 1000px;

}
.inputBox {
    width: 100%;
   /* width: 8rem;  */
}
.navigatorIcon {
    color: #D70F64;
}
.btn {
    width: 17rem;
    border-radius: 0.5rem;
    background:#D70F64;
    color: white;
    font-weight: 900;
}

</style>