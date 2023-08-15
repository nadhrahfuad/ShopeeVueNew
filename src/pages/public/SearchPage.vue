<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import TitleSection from '@/components/sections/TitleSection.vue'
import SearchBar from '@/components/elements/SearchBar.vue'
import RecentSearches from '@/components/sections/search/RecentSearches.vue'

</script>

<template>
    <WhiteContainer class="bg">     
            <TitleSection />
            <SearchBar class="searchbar1"/>
            <RecentSearches/>
    </WhiteContainer>
</template>


<style scoped>
.searchbar1{
    display: flex;
    justify-content: flex-end;
    width: 303px;
    margin-top: -45px;
    
}
</style>