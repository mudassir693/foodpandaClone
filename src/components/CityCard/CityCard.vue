<template >
    <div class="main relative cursor-pointer my-2">
        <img class="img" :src="img" alt="">
        <div class="header opacity-50 hidden ">{{CityName.charAt(0)}}</div>
        <div class="textContainer ">
            
            <div class="flex justify-between items-center flexWrapper">
                <div class="cityname mx-5 text-white">
                    {{CityName}}
                </div>
                <div class=" py-2 px-4 arrowContainer">
                    <i class="arrow text-light text-2xl text-white fa-solid fa-arrow-right"></i>
                </div>
                
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props:['CityName','img']
    
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
.main:hover .header {
    display:block;
}
.main:hover .arrowContainer {
    visibility:visible;
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
    bottom: 130px;
    /* opacity: 0.8; */
    left: -20px;
    z-index: 1;
    font-size: 200px;
    line-height:104px;
    color: #d70f64;
    font-weight: 900;
     transition: all 200ms ease-in-out;

}
.cityname {
    font-size: 1.5rem;
    position: absolute;
    left: -0.2rem;
    bottom: .70rem;
    font-weight: 900;
}
.arrowContainer {
    background:#d70f64;
    border-radius: .5rem;
     transition: all 200ms ease-in-out;
     visibility:hidden;
     position: absolute;
     right: 0;
     bottom: 0rem;
}
.arrow {
   
}
.flexWrapper {
    position: relative;
    z-index: 200;
}
</style>