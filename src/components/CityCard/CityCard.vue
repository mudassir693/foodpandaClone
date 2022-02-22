<template >
    <div class="main relative">
        <img class="img" src="https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Karachi.jpg?width=400&height=400" alt="">
        <div class="header">K</div>
        <div class="textContainer ">
            
            <div class="flex justify-between items-center flexWrapper">
                <div class="cityname mx-5 text-white">
                    Karachi
                </div>
                <div class=" border border-red-500  p-3 px-4 arrowContainer">
                    <i class="arrow text-light text-2xl text-white fa-solid fa-arrow-right"></i>
                </div>
                
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
    height: 272px;
    width: 216px;
    overflow:hidden;

    /* background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url('https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Karachi.jpg?width=400&height=400'); */
}
.main:hover .img {
    transform:scale(1.2);
}
.img {
    /* position: absolute;
    top: 0;
    left: 0; */
    width:100%;
    height: 100%;
    transition: all 200ms ease-in-out;
    object-fit: cover;
}
.textContainer {
    position: absolute;
    bottom: 0px;
    /* background-color:pink; */
    width: 100%;
}
.wrapper {
    width: 100%;
    /* background-color:pink; */
}
.header {
    position: relative;
    bottom: 100px;
    opacity: 0.8;
    left: -20px;
    z-index: 1;
    font-size: 200px;
    line-height:104px;
    color: #d70f64;
    font-weight: 900;

}
.cityname {
    
}
.arrowContainer {
    background:#d70f64;
    border-radius: .5rem;
}
.arrow {
   
}
.flexWrapper {
    position: relative;
    z-index: 200;
}
</style>