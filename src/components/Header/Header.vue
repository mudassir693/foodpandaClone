<template>
    <div class="main  flex justify-between py-3 bg-white  px-3 h-400  items-center max-w-7xl mx-auto text-center">
         <div class="logoContainer  text-2xl ">
             <img class="logo inline-block w-11 h-11 rounded-full" src="https://assets.foodora.com/c1d829a/img/favicon/foodpanda/apple-touch-icon-114x114.png?c1d829a" alt="">
             <span style="font-weight:600;color:#D70F64">
                 foodpanda
             </span>
         </div>
         <div style="height:100%" class="navigationSection text-1xl font-bold flex justify-between items-center">
             <div class="divider"></div>
             <div class="eachNavContainer cursor-pointer">
                 EN
             </div>
             <div class="divider"></div>
             <div class="navSection ">

             
                <div class="eachNavContainer flex items-center cursor-pointer">
                    <div class="avatarContainer">
                        <img class="inline-block h-8 w-8 rounded-full ring-2 ring-white" src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt=""/>
                    </div>
                    <span class="mx-2">
                        Mudassir Siddiqui
                    </span>
                    <span v-if="!isActive" @click="showOptions" style="font-weight:100;color:#D70F64;">
                        <i class="fa-solid fa-angle-down text-2xl"></i>
                    </span>
                    <span v-if="isActive" @click="showOptions" style="font-weight:100;color:#D70F64;">
                        <i class="fa-solid fa-angle-up text-2xl"></i>
                    </span>
                </div>

                <div v-show="isActive" style="width:125%" class=" py-1 links border text-grey-500 text-left rounded-md">
                    <div class="eachLink py-2 px-3 cursor-pointer ">My orders</div>
                    <div class="eachLink py-2 px-3 cursor-pointer ">Profile</div>
                    <div class="eachLink py-2 px-3 cursor-pointer ">Vouchers</div>
                    <div class="eachLink py-2 px-3 cursor-pointer ">pandapay</div>
                    <div class="eachLink py-2 px-3 cursor-pointer ">Chellanges & rewards</div>

                </div>

             </div>

             <div class="divider"></div>
             <div class="eachNavContainer">
                 <div class="basketContainer text-2xl cursor-pointer">
                    <i style="color:#D70F64;" class="fa-solid fa-cart-shopping"></i>
                 </div>
             </div>
         </div>
    </div>
</template>

<script>
export default {

    data(){
        return {
            isActive:false
        }
    },
    methods:{
        showOptions(){
            this.isActive = !this.isActive
        }
    }

}
</script>

<style scoped>
.navSection {
    position:relative;
}
.links {
    z-index: 9999;
    position:absolute;
    background:white;
    left: -1.5rem;
    top: 3rem;
    
}
.eachLink {
    font-weight: 100;
    font-size: 1.2rem;
    user-select: none; 
    /* font-family: 'Open Sans Condensed', sans-serif; */
}
.eachLink:hover {
    font-weight: 100;
    font-size: 1.2rem;
    color: #D70F64;
    background:#f3f3f3;

}
.main {
    color:#5F5F5F;
    z-index: 999;
}
.navigationSection {
    width: 30%;
}
 .divider {
        width:1px;
        background-color:#A8B2BD;
        height: 30px;
    }   
</style>