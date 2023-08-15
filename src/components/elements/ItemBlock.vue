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
</style>