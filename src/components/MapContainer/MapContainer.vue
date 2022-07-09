<template>
    <div id="map" class="relative">
    </div>
</template>

<script>
import store from '@/store/index.js';
import mapboxgl from 'mapbox-gl'; 
import axios from 'axios'
import 'mapbox-gl/dist/mapbox-gl.css'; 
export default {
    data() {
    return {
      lat:store.state.lat,
      long:store.state.lon,
      accessToken:'pk.eyJ1IjoibXVoYW1tYWQtbXVkYXNzaXIiLCJhIjoiY2w1OWxlMnAxMGYwZjNjcDRzeWp5YnZtOSJ9.yovt1JF_3gAzGl2KAhK2qA',
      placeName:""
    };
  },
  props: ['setPlace'],



    mounted(){

        //  if (navigator.geolocation) {
        //         console.log('navigator is OK: ',store.state.lat)


        //     navigator.geolocation.getCurrentPosition(function(position) {

        //         console.log('cordinates: ,',position.coords.latitude);
        //         this.lat = position.coords.latitude;

        //     }, function(error) {
        //         console.log(error)

        //     });
        // } 

        console.log('it is triggered', this.$store.state.lon);
        mapboxgl.accessToken = this.accessToken;

        const map = new mapboxgl.Map({
            container: 'map',
            style: "mapbox://styles/mapbox/streets-v11",
            center: [this.long, this.lat],
            zoom: 13,
        })

        // this.addToMap(map)

        const marker1 = new mapboxgl.Marker({draggable: true})
            .setLngLat([this.long, this.lat])
            .addTo(map);




        console.log(marker1);

        let onDragEnd= async ()=> {
            const lngLat = marker1.getLngLat();
            console.log('marker moved:', lngLat)
            store.state.lat = lngLat.lat
            store.state.lon = lngLat.lng

            const resp = await axios.get(`https://api.mapbox.com/geocoding/v5/mapbox.places/${lngLat.lng},${lngLat.lat}.json?access_token=pk.eyJ1IjoibXVoYW1tYWQtbXVkYXNzaXIiLCJhIjoiY2w1OWxlMnAxMGYwZjNjcDRzeWp5YnZtOSJ9.yovt1JF_3gAzGl2KAhK2qA`)
            console.log('here is address: ', resp)
            // this.setPlace(resp?.data.features[0].place_name)
            this.$emit('setPlace',resp?.data.features[0].place_name );
        }

        marker1.on('dragend', onDragEnd);
    },

      methods:{
        addToMap:function(map){
        let marker = new mapboxgl.Marker()
                .setLngLat([67.1023104, 24.920064]).addTo(map);

            console.log(marker)
        }
  },
}
</script>

<style scoped>
#map {
    width: 100%;
    height: 100%;
}
.searchBoxContainer {


}

</style>