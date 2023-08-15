<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import InfoMyCartSection from '@/components/sections/mycart/InfoMyCartSection.vue'
import BottomNavigation from "@/components/navigations/BottomNavigation.vue";
</script>

<template>
    <WhiteContainer>
        <TitleSection title="My cart" />
        <InfoMyCartSection />
        <BottomNavigation class="navbar"/>
    </WhiteContainer>
</template>

<style scoped>
.navbar{
    margin-top: 214px;
}
</style>