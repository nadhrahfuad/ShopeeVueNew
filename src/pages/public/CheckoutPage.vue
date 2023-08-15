<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import CustomerInformation from '@/components/sections/checkout/CustomerInformation.vue'


</script>

<template>
    <WhiteContainer>
        <TitleSection title="Checkout" />
        <CustomerInformation firstname="Luka" lastname="Marjanovic" street="221b Baker St, Marylebone" city="London" country="United Kingdom"/>
        
    </WhiteContainer>
</template>

<style scoped>
.navbar{
    margin-top: 214px;
}
</style>