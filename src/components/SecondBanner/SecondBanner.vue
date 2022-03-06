<template >
    <div :style="{'background-image':`url(${bgImage})`}" class="main  mx-auto bg-red-100">
        <div class="container max-w-7xl mx-auto">
            <div class="cardTop">

            
            <div class="absolute md:relative md:block card bg-white  p-5">
                <div class="wrapper  m-3">
                <div class="heading my-2 text-[#333333]">
                    {{heading}}
                </div>
                <div class="pera my-4">
                    <div v-if="pera1" class="peragraph text-[#707070] my-3">
                        {{pera1}}
                    </div>
                    <div v-if="pera2" class="peragraph text-[#707070] my-3">
                       {{pera2}}
                    </div>
                    <div v-if="pera3" class="peragraph text-[#707070] my-3">
                       {{pera3}}
                    </div>
                </div>


                 <div class="btnContainer md:text-right ">
                     <div class="hiddn  md:my-5"> j</div>
                    <span class="btn text-white cursor-pointer">
                        Get started
                    </span>
                </div>
               
                </div>
                

            </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props:['bgImage','heading','pera1','pera2','pera3']
    
}
</script>
<style scoped>
.main {
    max-height: 500px;
    position: relative;
    height: 70vh;
    /* z-index: 999; */
    /* background-image: url('../../assets/resturant.webp'); */
    background-position:center center;
    background-repeat:no-repeat;
    background-size: cover;
    margin-bottom:7rem;
    /* transform: scale(1); */
}
.btn {
    background: #D70F64;
    border-radius: 0.5rem;
    padding: 1.3rem 5rem;
    font-weight: 700;
    font-size: 1rem;
}
.btnContainer {
    position: absolute;
        bottom: 2rem;
        right: 0rem;
}
.hiddn {
    visibility: hidden;
}
.heading {
    font-size: 1.5rem;
    font-weight: 300;
}
.peragraph {
    font-size: 1.2rem;
    font-weight: 300;
}
.wrapper {
    height: 100%;
    position: relative;
}

.card {
    background-color: white;
    height: 400px;
    /* min-height: 75%; */
    width: 50%;
    /* max-height: 400px; */
    border-radius: 2px;
    position: absolute;
    top: 37%;
    /* transform: translateY(40%); */
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.container {
    height: 100%;
    position: relative;
}

@media screen and (max-width: 640px) {
    .main {
        max-height: 500px;
        position: relative;
        height: 35vh;
        /* z-index: 999; */
        /* background-image: url('../../assets/resturant.webp'); */
        background-position:center center;
        background-repeat:no-repeat;
        background-size: content;
        margin-bottom:19rem;
        /* transform: scale(1); */
    }
    .btn {
        background: #D70F64;
        border-radius: 0.5rem;
        font-weight: 700;
        font-size: 1rem;
         width: 100%;
         height: 2.8rem;
    }   
    .btnContainer {
        position: relative;
        bottom: 0;
        width: 100%;
         height: 100%;
    }
    .btnContainer {
       /* position: relative; */
        /* bottom: 2rem;
        right: 0rem; */
    }
    .card {
            position: absolute;
        top:80%;
        left:50%;
        width: 95%;
        transform: translateX(-50%);
        height: fit-content;
    }
    .heading {
        font-size: 1.2rem;
        font-weight: 200;
    }
    .peragraph {
        font-size: .8rem;
        font-weight: 100;
    }
}
</style>