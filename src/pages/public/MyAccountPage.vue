<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import BottomNavigation from "@/components/navigations/BottomNavigation.vue";
import AccountInfo from '@/components/content/AccountInfo.vue';

</script>

<template>
    <div class="back">
        <WhiteContainer class="bg">
            <TitleSection title="My account"/>
            <AccountInfo/>
            <BottomNavigation/>
        </WhiteContainer>
    </div>
</template>

<style scoped>


.back{
    width: 375px;
    height: 812px;
    background-color: #FFF;
    border-radius: 20px;
}
</style>

