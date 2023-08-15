<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import OrderSuccessSection from '@/components/sections/ordersuccess/OrderSuccessSection.vue'
// import ButtonGreyVue from '@/components/elements/ButtonGrey.vue';

</script>

<template>
    <WhiteContainer>
        <OrderSuccessSection maintext="Order success!"
            subtext="Your order has been placed successfully! For more details, go to my orders." />
    </WhiteContainer>
</template>