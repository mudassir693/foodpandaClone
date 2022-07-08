<template>

    <div id="map" class="relative">
    </div>
</template>

<script>
import store from '@/store/index.js';
import mapboxgl from 'mapbox-gl'; 
import 'mapbox-gl/dist/mapbox-gl.css'; 
export default {
    data() {
    return {
      lat:store.state.lat,
      long:store.state.lon,
      accessToken:'pk.eyJ1IjoibXVoYW1tYWQtbXVkYXNzaXIiLCJhIjoiY2w1OWxlMnAxMGYwZjNjcDRzeWp5YnZtOSJ9.yovt1JF_3gAzGl2KAhK2qA',
    };
  },



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

        function onDragEnd() {
            const lngLat = marker.getLngLat();
            coordinates.style.display = 'block';
            coordinates.innerHTML = `Longitude: ${lngLat.lng}<br />Latitude: ${lngLat.lat}`;
        }
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