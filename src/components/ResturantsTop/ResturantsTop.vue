<template >
    <div class="main flex  max-w-7xl mx-auto bg-white pt-10">
       <div @click="setActive('delivery')" :class="isActive=='delivery'?'active':''" class="eachCard cursor-pointer relative  flex justify-start p-5 items-end ">
           <div class="text text-xl  text-[#D70F64]">
                Delivery
           </div>
           <div class="imageContainer absolute">
               <img src="https://images.deliveryhero.io/image/foodpanda/vertical-switcher/pk/restaurants.png" alt="">
           </div>
           <div class="bottomLine absolute"></div>
       </div>

       <div @click="setActive('pick-up')" :class="isActive=='pick-up'?'active':''" class="eachCard mx-4 text-xl cursor-pointer relative  flex justify-start p-5 items-end ">
           <div class="text">
                Pick-Up
           </div>
           <div class="imageContainer absolute">
               <img src="https://images.deliveryhero.io/image/foodpanda/vertical-switcher/pk/pickup.png" alt="">
           </div>
           <div class="bottomLine absolute"></div>
       </div>
       <!-- <div class="eachCard bg-yellow-200">
           Delivery
       </div> -->
    </div>
</template>
<script>
export default {

    data(){
        return {
            isActive:'delivery'
        }
    },
    methods: {
        setActive: function(parameter){
            this.isActive =  parameter
            // console.log("Hello Haider: ", parameter);
        }
    }
    
}
</script>
<style scoped>
    .active {
        font-weight: 700;
        box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
        border-bottom: 2px solid #D70F64;
        /* background-color: lightgrey; */
    }
    .eachCard {
        height: 3.5rem;
        width: 18rem !important;
        overflow: hidden;
        /* background-color:lightgrey; */
        /* border-bottom: 4px solid red; */
    }
    .imageContainer{
        transform: scale(1.57);
        right: 2rem;
        top:-1.5rem;
        object-fit: contain;
    }
    .bottomLine {
        width:100%;
        left: 0rem;
        bottom: 0rem;
        height: 1px;
        /* background-color:#D70F64 */
    }
</style>