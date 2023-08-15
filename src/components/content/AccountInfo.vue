<!-- @/components/sections/myaccount/EditAccountSection.vue -->
<script setup>

defineProps({
    itemname: {
        type: String,
        default: 'Product name here'
    },

    currency: {
        type: String,
        default: 'currency'
    },

    price: {
        type: String,
        default: 'price'
    },

    oldprice: {
        type: String,
        default: 'oldprice'
    },

    sold: {
        type: String,
        default: 'sold'
    },
})


import EditAccountSection from '@/components/sections/myaccount/EditAccountSection.vue'
import DigitalPurchases from '@/components/sections/myaccount/DigitalPurchases.vue'
import MyPurchasesOrange from '@/components/sections/myaccount/MyPurchasesOrange.vue'
import EmptyContainerSection from '@/components/sections/myaccount/EmptyContainer.vue'

</script>


<template>
   <div class="accountinfo-container">
    <EditAccountSection firstname="Adji" lastname="Rahadian" text=""/>
    <DigitalPurchases/>
    <MyPurchasesOrange currency="Rp." shopeepayprice="4.982.000" coin="928.300" spaylaterprice="10.620.912" voucher="92"/>
    <EmptyContainerSection/>
    
   
    </div>
</template>


<style scoped>

</style>