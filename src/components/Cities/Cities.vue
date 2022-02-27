<template>
    <div>
        <div  class="mainn text-3xl max-w-7xl mx-auto md:grid md:grid-cols-4 lg:grid lg:grid-cols-5">
            <div v-for="city in cityArray" :key="city.cityNam" class="flex justify-center items-between">
                <CityCard :CityName="city.CityName" :img="city.Img" />
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
                {CityName:"Karachi",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Karachi.jpg?width=400&height=400"},
                {CityName:"Lahore",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Lahore.jpg?width=400&height=400"},
                {CityName:"Islamabad",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Islamabad.jpg?width=400&height=400"},
                {CityName:"Rawalpindi",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Rawalpindi.jpg?width=400&height=400"},
                {CityName:"Faislabad",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Faisalabad.jpg?width=400&height=400"},
                {CityName:"Multan",Img:"https://images.deliveryhero.io/image/foodpanda/city-tile-pk/Multan.jpg?width=400&height=400"},
                {CityName:"Murree",Img:"https://images.deliveryhero.io/image/fd-pk/city-tile/city-tile-Murree.jpg?width=400&height=400"},
                {CityName:"Quetta",Img:"https://images.deliveryhero.io/image/fd-pk/city-tile/city-tile-Quetta.jpg?width=400&height=400"},
                {CityName:"Sheikhupura",Img:"https://images.deliveryhero.io/image/fd-pk/city-tile/city-tile-Sheikhupura.jpg.jpg?width=400&height=400"},
                {CityName:"Abottabad",Img:"https://images.deliveryhero.io/image/fd-pk/city-tile/city-tile-Abottabad.jpg?width=400&height=400"}
            ]
        }
    }
}
</script>

<style scoped>
    .mainn {
        margin-bottom:5rem;
    }
</style>