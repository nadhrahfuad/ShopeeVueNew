<script setup>
defineProps({
    storename: {
        type: String,
        default: 'storename'
    },

    location: {
        type: String,
        default: 'location'
    },

    active: {
        type: String,
        default: 'mins'
    }
})

import ProductRatingSection from './ProductRatingSection.vue';
import ButtonOrange from '@/components/elements/ButtonOrange.vue';

</script>


<template>
   <div class="store-container">
        <div class="storeelements">
            <div class="storelogo">

                <div class="logoimg">
                    <img src="@/assets/images/svgs/storelogo.svg" alt="" class="logo">
                </div>

                <div class="malltag">
                    <div class="shopeemall">
                        <span class="taglabel">
                            SHOPEE MALL
                        </span>
                    </div>
                </div>

            </div>
            <div class="storedescription">
                <div class="storename-container">

                    <div class="storename">
                        <span class="name">
                            @{{ storename }}
                        </span>
                    </div>

                    <div class="locandactivestatus">
                        <div class="location-container">
                            <div class="iconcontainer">
                                <img src="@/assets/images/svgs/locationicon.svg" alt="" class="locationicon">
                            </div>
                            <div class="storelocation">
                                <span class="location">
                                    {{ location }}
                                </span>
                            </div>
                        </div>
                        <div class="active-container">
                            <div class="activestatus">
                                <span class="active">
                                    Aktif {{ active }} Menit yang lalu
                                </span>
                            </div>
                        </div>
                    </div>

                </div>
            
                <div class="visitbtn">
                    <button class="visit">
                        <span class="btnlabel">
                            Visit Store
                        </span>
                    </button>
                </div>
            </div>
            
        </div>
        <ProductRatingSection count="RB" product="2,4" rating="4.8" chat="100"/>
        <div class="button-container">
            <ButtonOrange link="/search" text="Add to cart" />
        <CameraBtn/>
    </div>
    </div>
</template>

<style scoped>
.store-container{
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 357px;
    height: 293px;
    border-radius: 19px 19px 0 0 ;
    background: #FFF;
    box-shadow: -5px 15px 35px 0px rgba(35, 35, 35, 0.10);
}
.storeelements{
    display: flex;
    justify-content: center;
    margin-top: 8px;
    /* border: red 2px solid; */
}

.storedescription{
    display: flex;
    height: 74px;
    width: 249px;
    justify-content: space-between;
    align-items: center;
}

.storename-container{
    display: flex;
    flex-direction: column;
}

.locandactivestatus{
    display: flex;
    flex-direction: row;
    height: 10px ;
    align-items: center;
    width: 115px;
    justify-content: space-between;
    margin-top: 4px;
    
}


.storelocation{
    display: flex;
    width: 40px;
}

.location-container, .storelocation, .activestatus {
    display: flex;
    align-items: center;
    height: 10px;
    
}

.iconcontainer{
    display: flex;
    margin-right: 2px;
    align-items: center;
    justify-content: center;
}

.malltag{
    display: flex;
    position: absolute;
    margin-top: -23px;
}
.shopeemall{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 74px;
    height: 13px;
    border-radius: 2px;
    background: #EB001B;
    
}
.visitbtn{
    display: flex;
    height: 22px;
    align-items: center;
}
.button-container{
    display: flex;
    justify-content: center;
    margin-top: 16px;
    margin-bottom: 25px;
}
.taglabel{
    color: #FFF;
    font-family: Shopee 2021;
    font-size: 10px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
}

.name{
    width: 125px;
    color: #1F1F1F;
    font-family: Montserrat;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.location{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 6px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
}

.active{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 5px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
}

button{
    border: none;
    background-color: none;
    background: none;
}
.visit{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 86px;
    height: 17px;
    flex-shrink: 0;
    border-radius: 2px;
    border: 0.5px solid #1F1F1F;
    cursor: pointer;
}
.btnlabel{  
    width: 69px;
    color: #1F1F1F;
    text-align: center;
    font-family: Montserrat;
    font-size: 11px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}


</style>