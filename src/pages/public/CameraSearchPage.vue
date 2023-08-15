<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import SearchDialSection from '@/components/sections/camerasearch/SearchDialSection.vue'
import CameraFooterSection from '@/components/sections/camerasearch/CameraFooterSection.vue'

</script>

<template>
    <WhiteContainer class="bg">
        <TitleSection />
        <SearchDialSection/>
        <CameraFooterSection/>
    </WhiteContainer>
</template>


<style scoped>
.bg{
    background-image: url('@/assets/images/pictures/productsearch.png');
    background-repeat: no-repeat;
   
}
</style>