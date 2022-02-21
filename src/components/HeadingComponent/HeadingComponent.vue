<template >
    <div>
       <div class="main max-w-7xl mx-auto text-left flex items-center">
           <div class="mainHeader">
               {{Header}}
           </div>
           <div class="desc my-2">
               {{Desc}}
           </div>
        </div> 
    </div>
</template>
<script>
export default {

    props:['Header','Desc']
    
}
</script>
<style scoped>
 .main {
     /* background: red !important; */
     position: relative;
     /* height: 15vh; */
     height: 100px;
     /* overflow-x: hidden */
 }   
 .mainHeader {
     position: absolute;
    font-size: 10rem;
    font-weight: 900;
    color: lightgray;
 }
 .desc {
     position: absolute;
     bottom: -0.38rem; 
     font-size: 1.7rem;
     color: #333333;
     font-weight: 100;
 }
</style>