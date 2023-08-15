<script setup>

defineProps({
    itemname: {
        type: String,
        default: 'Product name here'
    },

    currency: {
        type: String,
        default: 'currency'
    },

    price: {
        type: String,
        default: 'price'
    },

    oldprice: {
        type: String,
        default: 'oldprice'
    },

    sold: {
        type: String,
        default: 'sold'
    },
})

import RatingIcon from '@/components/sections/mywishlist/RatingIcon.vue'

</script>


<template>
   <div class="itemcard-container">
        <div class="descriptionelements">
            <div class="itemname">
                <span class="name">
                    {{ itemname }}
                </span>
            </div>
            <div class="price-container">
                <div class="currentprice">
                    <span class="currency">
                        {{currency}}
                    </span>
                    <span class="price">
                        {{price}}
                    </span>
                </div>
                <div class="oldprice-container">
                    <div class="line">

                    </div>
                    <div class="crossed">
                        <span class="crossedcurrency">
                            {{currency}}
                        </span>
                        <span class="oldprice">
                            {{oldprice}}
                        </span>
                    </div>
                </div>
            </div>
            <div class="cardfooter">
                <div class="rating-container">
                    <RatingIcon/>
                    <span class="rating">
                        4.9
                    </span>
                </div>
                <div class="sold-container">
                    <span class="soldtxt">{{ sold }} Terjual</span>
                </div>
            </div>
        </div>
   
   
    </div>
</template>


<style scoped>

.itemcard-container{
    display: flex;
    width: 357px;
    height: 117px;
    flex-shrink: 0;
    border-radius: 19px;
    background: #FFF;
    box-shadow: -5px 15px 35px 0px rgba(35, 35, 35, 0.10);
    justify-content: center;
    margin-top: 6px;;
}

.descriptionelements{
    display: flex;
    width: 326px;
    flex-direction: column;
    margin-top: 17px ;
    
}

.cardfooter{
    display: flex;
    height: 15px;
    align-items: center;
    /* border: black 2px solid; */
    justify-content: space-between;
    margin-top: 11px;

}

.rating-container, .sold-container{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 15px;
}

.currentprice{
    display: inline-block;
    /* border: #000 solid 2px; */
}

.crossed{
    display: flex;
    align-items: flex-end; 
    /* border: red solid 2px; */
}

.itemname{
    display: flex;
    margin-bottom: 15px;
}

.name{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.currency{
    color: #FF5F00;
    font-family: Montserrat;
    font-size: 9px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.price{
    color: #FF5F00;
    font-family: Montserrat;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.crossedcurrency{
    color: #B4B4B4;
    font-family: Montserrat;
    font-size: 5px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-bottom: 2px;
}

.oldprice{
    color: #B4B4B4;
    font-family: Montserrat;
    font-size: 10px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.rating-container{
    display: flex;
    align-items: center;
}

.rating{
    color: #000;
    font-family: Montserrat;
    font-size: 10px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-left: 1px;
}

.soldtxt{
    color: #000;
    font-family: Montserrat;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.line{
    display: flex;
    position: absolute;
    width: 53px;
    height: 1px;
    flex-shrink: 0;
    background-color: #B4B4B4;
    margin-top: 7px;
}

</style>