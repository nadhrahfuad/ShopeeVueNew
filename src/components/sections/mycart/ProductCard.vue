<script setup>

import { ref } from 'vue'

const counter = ref(1)

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
    }
})

</script>


<template>
   <div class="item-container">
        <div class="itempic">
            <img src="@/assets/images/pictures/shoe.png" alt="" class="pic">
        </div>
        <div class="itemdesc">
            <div class="itemname">
                <span class="name">
                    {{ itemname }}
                </span>
            </div>
            <div class="itemprice">
                <span class="currency">
                    {{ currency }}
                </span>
                <span class="price">
                    {{ price }}
                </span>
            </div>
            <div class="itemcount">
                <button class="decrease" @click="counter--">
                    <span class="minus">
                        -
                    </span>
                </button>
                <div class="itemamount-container">
                    <span class="itemamount">{{ counter }}</span>
                </div>
                <button class="increase" @click="counter++">
                    <span class="plus">
                        +
                    </span>
                </button>

            </div>

        </div>
   
  </div>
</template>


<style scoped>
.item-container{
    display: flex;
    width: 303px;
    height: 112px;
    flex-shrink: 0;
    border-radius: 14px;
    align-items: center;
    border: 0.5px solid #D5DDE0;
}


.itemdesc{
    display: flex;
    flex-direction: column;
}
.itempic{
    display: flex;
    width: 92.593px;
    height: 100px;
    flex-shrink: 0;
    border-radius: 7.407px;
    border: 0.37px solid #D5DDE0;
    background: var(--grey-3, #F7F8F9);
    align-items: center;
    justify-content: center;
    margin-left: 6px;
    margin-right: 13.41px;
    
}

.pic{
    width: 92.593px;
    height: 100px;
    border-radius: 7.407px;
}

.itemname{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.currency, .price, .cents{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    word-spacing: none;
}

.itemcount{
    display: flex;
    margin-top: 12px;
}

button{
    border: none;
    background-color: none;
    background: none;
}

.increase, .decrease{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.itemamount-container{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 23px;
    height: 23px;
    flex-shrink: 0;
    border-radius: 4px;
    border: 1px solid #D5DDE0;
}

.itemamount{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: normal; 
}
</style>