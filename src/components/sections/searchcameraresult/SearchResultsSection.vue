<template>
    <div class="ItemsFoundContainer">
        <div class="itemsfound">
            <div class="countitemsfound">
                <span class="count">
                    {{ numberofitemsfound }} items found
                </span>
            </div>
            <ItemBlock class="itembox" itemname="Nike Free Metcon 3" currency="$" price="160.00"/>
            <ItemBlock class="itembox" itemname="Nike Free Metcon 3" currency="$" price="160.00"/>
            <ItemBlock itemname="Nike Free Metcon 3" currency="$" price="160.00"/>
        </div>

       
    </div>
    <Slider/>
    
</template>

<script setup>
defineProps({
    numberofitemsfound: {
        type: String,
        default: 'numberofitems'
    }
})

import Slider from '@/components/elements/Slider.vue'
import ItemBlock from '@/components/elements/ItemBlock.vue'
</script>

<style scoped>
.ItemFoundContainer {
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    width: 100%;
}

.itemsfound{
    display: flex;
    position: absolute;
    flex-direction: column;
    align-items:center;
    width: 375px;
    height: 466px;
    margin-left: -188px;
    border-radius: 19px;
    margin-top: 273px;
    background-color: #FFF;
    /* border: black solid 1px; */
}

.countitemsfound{
    display:flex;
    margin-top: 14px;
}

.count{
    display: flex;
    color: #97ADB6;
    font-family: Montserrat;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-bottom: 14px;
}
.itembox{
    display: flex;
    margin-bottom: 16px;
}



</style>