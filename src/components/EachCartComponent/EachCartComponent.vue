<template>
  <div class="mainn flex justify-between items-start my-2 px-2 py-2 cursor-pointer">
    <div class="nameContainer theme text-base font-medium">
        Pizza Fajita
    </div>
    <div class="right flex justify-start items-end flex-col">
        <div class="price text-gray-500 font-thin">
            Rs. 1024
        </div>
        <div class="flex justify-end items-center my-1 shadoww p-2">
            <i class="fa-solid fa-trash-can theme"></i>
            <span class="qty text-base mx-2 theme">1</span>
            <i class="fa-solid fa-plus text-white theme"></i>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.mainn {
    width:100%;
}
.mainn:hover .shadoww{
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.theme {
    color:#DA0060;
}
.shadoww {
    transition: all 0.2s ease-in-out;
    border: none;
}
</style>