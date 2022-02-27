<template>
    <div>
        <div  class="mainn text-3xl max-w-7xl mx-auto bg-red-100 grid grid-cols-5 ">
            <div v-for="city in cityArray" :key="city.cityNam" class="flex justify-center items-between">
                <CityCard :CityName="city.CityName" />
            </div>
        </div>
    </div>
</template>

<script>
import CityCard from '../CityCard/CityCard.vue'
export default {
    components:{
        CityCard,
    },
    data(){
        return {
            cityArray:[
                {CityName:"Karachi",Img:""},
                {CityName:"Islamabad",Img:""},
                {CityName:"Quetta",Img:""},
                {CityName:"Peshawar",Img:""},
                {CityName:"Haidrabad",Img:""}
            ]
        }
    }
}
</script>

<style scoped>
    
</style>