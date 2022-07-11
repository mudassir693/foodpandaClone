<template>
  <div class="main py-10 px-3">
    <div class="wrapper mt-10 mb-5">
        <div class="topContainer text-center">
            <div class="my-5">
                <i class="fa-solid fa-truck-fast theme text-2xl"></i>
                <div class="text-gray-500 text-base">5 min</div>
            </div>
            <div class="my-2 text-base font-bold ">
                Your Order Pizza Max - Nazimabad, Karachi. 
            </div>
        </div>
        <div class="itemContainer">
            <div class="eachItem">
                <EachCartComponent />
                <EachCartComponent />
            </div>
        </div>

        <div class="saperator"></div>
        <div class="my-3">
            <div class="flex justify-between items-center">
                <div class="text-gray text-base font-thin text-gray-500">Subtotal</div>
                <div class="text-gray text-base font-thin text-gray-500">Rs. 0</div>
            </div>
            <div class="flex justify-between items-center mt-2">
                <div class="text-gray text-base font-medium ">Total(Incl. GST)</div>
                <div class="text-gray text-base font-medium ">Rs. 0</div>
            </div>
            <div class="my-2">
                <div class="submit cursor-pointer bg-theme text-white text-base flex justify-center items-center py-2 rounded-lg">
                    <span>
                        Go to checkout
                    </span>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import EachCartComponent from '../EachCartComponent/EachCartComponent.vue';
export default {
    components: { EachCartComponent }
}
</script>

<style scoped>
.main{
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    z-index: 999;
    min-height: calc(100vh - 40px);
}
.theme{
    color: #DA0060;
}
.bg-theme{
    background: #DA0060;
}
.saperator {
    height:1px;
    width: 100%;
    background-color: gray;

}
</style>