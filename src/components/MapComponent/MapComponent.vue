<template>
  <div v-if="this.$store.state.mapContainer==true" class="main flex justify-center items-center ">
    <div class="modal mx-auto my-auto bg-white">
        <div class="mapheader text-2xl font-bold py-5 px-5 flex justify-between items-center">
            <span>
                Is this your exact location?
            </span>
             <span @click="closeModal" class="text-gray-700 cursor-pointer">
                X
            </span>
        </div>
        <div  class="w-full mapContainerr bg-red-500">
            <MapContainer class="mapContainer" />
        </div>
        <div class=" py-5 w-full">
            <!-- <div class="inputContainer border-2 rounded-lg border-gray-500 mx-auto py-1  flex justify-center items-center">
                <input class="w-full py-1 outline-none rounded-lg px-3" v-model="inputFeild" type="text" name="" id="">
                <i @click="addressTyped" class="fa-solid fa-paper-plane cursor-pointer mr-3"></i>
            </div> -->
            <div class="submitBtn mx-auto cursor-pointer my-1 py-2 rounded-lg flex justify-center items-center ">
               <span class="text-md font-bold "> Confirm </span>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import store from '@/store/index.js'
import MapContainer from '../MapContainer/MapContainer.vue'
export default {
    components: {
        MapContainer
    },
    data(){
        return {
            inputFeild:''
        }
    },
    methods:{
        addressTyped:function(){
            console.log(this.inputFeild);
        }, 
        closeModal(){
            store.state.mapContainer = false
        }
    }
}
</script>

<style scoped>
.main {
    position:fixed;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100vw;
    background-color:black;
   background: rgba(0, 0, 0, .5);
    z-index: 10000;
}
.modal {
    width: 40%;
    height: fit-content;
    margin: auto auto;
    /* background:pink; */
}
.mapContainer {
    width: 100%;
    height: 100%;
}
.mapContainerr{
    width: 100%;
    height: 50vh;
}
.inputContainer {
    width: 90%;

}
.submitBtn {
    width: 90%;
    background-color: #DA0060;
    color: #FFFFFF;

}


</style>