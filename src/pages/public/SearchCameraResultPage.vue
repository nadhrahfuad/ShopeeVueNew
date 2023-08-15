<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import SearchResultSection from '@/components/sections/searchcameraresult/SearchResultsSection.vue'

</script>

<template>
    <WhiteContainer class="bg">
        <TitleSection />
        <SearchResultSection numberofitemsfound="3"/>
    </WhiteContainer>
</template>


<style scoped>
.bg{
    background-image: url('@/assets/images/pictures/camsearchbg.png');
    background-repeat: no-repeat;
}
</style>