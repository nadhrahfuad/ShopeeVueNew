<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import PaymentMethodContent from '@/components/content/PaymentMethodContent.vue'
import Slider from '@/components/elements/Slider.vue'


</script>

<template>
    <WhiteContainer>
        <TitleSection title="Payment method" />
        <PaymentMethodContent/>
        <Slider/>
    </WhiteContainer>
</template>

<style scoped>
.navbar{
    margin-top: 214px;
}
</style>