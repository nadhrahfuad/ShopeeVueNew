<script setup>
import ButtonOrange from '@/components/elements/ButtonOrange.vue'
import ProductCard from '@/components/sections/mycart/ProductCard.vue'
import SearchBarCart from '@/components/sections/mycart/SearchBarCart.vue'
import CodeVoucherSection from '@/components/sections/mycart/CodeVoucherSection.vue'
import TotalSection from '@/components/sections/mycart/TotalSection.vue'

defineProps({
    text: {
        type: String,
        default: 'Add more products to your cart'
    },

    signInLink: {
        type: String,
        default: '/'
    },

    forgotPasswordLink: {
        type: String,
        default: '/'
    },
    currency: {
        type: String,
        default: 'currency'
    },
    price: {
        type: String,
        default: 'price'
    },

})


</script>


<template>
    <div class="info-container">
        <div class="text-container">
            <span>{{ text }}</span>
        </div>
        <SearchBarCart/>

        <div class="product-container">
            <ProductCard itemname="Nike React Miler" currency="$" price="170.00" class="product1"/>
            <ProductCard itemname="Nike Air Max 270" currency="$" price="112.00"/>
        </div>

        <CodeVoucherSection/>

        <TotalSection currency="$" price="282.00"/>

        <ButtonOrange link="/checkout" text="Checkout" class="button" />

    </div>
</template>

<style scoped>

.info-container {
    margin-top: 16px;
    width: 303px;
    height: 451px;
    /* background-color: rgb(22, 98, 98); */
}

.text-container {
    width: 303px;
    height: 48px;
    display: flex;
    align-items: flex-start;
    color: #3E4958;
    ;
}


.text-container>span {
    font-family: Roboto;
    font-size: 13px;
    font-weight: 400;
    line-height: 24px;
    letter-spacing: 0px;
    text-align: left;
}

.product1{
    margin-bottom: 16px;
}

.product-container{
    display: flex;
    flex-direction: column;
    margin-top: 32px;
    margin-bottom: 32px;
}

.total-container{
    display: flex;
    width: 303px;
    justify-content: space-between;
    margin-top: 47px;
}

.intotal, .price{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 16px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.button {
   margin-top: 26px;
}
</style>