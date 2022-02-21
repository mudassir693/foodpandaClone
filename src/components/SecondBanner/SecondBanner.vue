<template >
    <div class="main  mx-auto bg-red-100">
        <div class="container max-w-7xl mx-auto">
            <div class="cardTop">

            
            <div class="card bg-white  p-5">
                <div class="wrapper  m-3">
                <div class="heading my-2 text-[#333333]">
                    List your restaurant or shop on foodpanda
                </div>
                <div class="pera my-4">
                    <div class="peragraph text-[#707070] my-3">
                        Would you like millions of new customers to enjoy your amazing food and groceries? So would we!
                    </div>
                    <div class="peragraph text-[#707070] my-3">
                       It's simple: we list your menu and product lists online, help you process orders, pick them up, and deliver them to hungry pandas – in a heartbeat!
                    </div>
                    <div class="peragraph text-[#707070] my-3">
                       Interested? Let's start our partnership today!
                    </div>
                </div>


                 <div class="btnContainer   text-right">
                     <div class="hiddn my-5"> j</div>
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
    
}
</script>
<style scoped>
.main {
    max-height: 500px;
    position: relative;
    height: 70vh;
    /* z-index: 999; */
    background-image: url('../../assets/resturant.webp');
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
    position: relative;
        /* bottom: -5rem;
        right: 0rem; */
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
</style>