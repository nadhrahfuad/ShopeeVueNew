<script setup>

import Separator from '@/components/elements/Separator.vue'
import ButtonOrange from '@/components/elements/ButtonOrange.vue'
import Slider from '@/components/elements/Slider.vue'
import CameraBtn from '@/components/sections/search/CameraBtn.vue'

</script>


<template>
    <div class="recentsearches-container">
        <div class="title-container">
            <div class="headingelements">
                <div class="headingtitle">
                    <span class="recentsearchtitle">
                        Recent Searches
                    </span>
                </div>
                <button class="clear">
                    <span class="cleartxt">
                        Clear all
                    </span>
                </button>
            </div>
        </div>
        <Separator/>
        <div class="searchlist">
            <div class="searchitem">
                <span class="item">
                    Nike Air Max 270
                </span>
            </div>
            <Separator/>
            <div class="searchitem">
                <span class="item">
                    Erigo Store
                </span>
            </div>
            <Separator/>
            <div class="searchitem">
                <span class="item">
                    Screamous
                </span>
            </div>
            <Separator/>
            <div class="searchitem">
                <span class="item">
                    Musk by Ashley
                </span>
            </div>
            <Separator/>
            <div class="searchitem">
                <span class="item">
                    Adidas
                </span>
            </div>
            <Separator/>
            <div class="searchitem">
                <span class="item">
                    Hoodie
                </span>
            </div>
            <Separator/>
        </div>
    </div>

    <div class="button-container">
        <ButtonOrange link="/search" text="Search" />
        <CameraBtn/>
    </div>
    <Slider />
</template>

<style scoped>
.recentsearches-container{
    display: flex;
    flex-direction: column;
}
 .title-container{
    display:flex;
    flex-direction: row;
    width: 303px
}

.recentsearches-container{
    display: flex;
    margin-top: 16px;
}

.headingelements{
    display:flex;
    flex-direction: row;
    align-items: center;
    width: 100%;
    justify-content: space-between;
    margin-bottom: 11px;
}

.recentsearchtitle{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.clear{
    display: flex;
    width: 73px;
    height: 36px;
    flex-shrink: 0;
    border-radius: 7px;
    border: 0.5px solid #D5DDE0;
    background: #F7F8F9;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

.cleartxt{
    color: #D5DDE0;
    font-family: Montserrat;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.searchlist{
    display: flex;
    width: 303px;
    flex-direction: column;
}

.searchitem{
    display: flex;
    flex-direction: column;
    margin-top: 21px;
    margin-bottom: 20px;
}

.item{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
   
}

.button {
    width: 224px;
    height: 60px;
}

.button-container{
    display: flex;
    flex-direction: row;
    margin-top: 141px;
    width: 303px;
    justify-content: space-evenly;
}
</style>