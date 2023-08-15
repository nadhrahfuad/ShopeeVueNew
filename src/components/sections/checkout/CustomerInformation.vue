<script setup>

import Separator from '@/components/elements/Separator.vue'
import MasterCardSection from '@/components/sections/checkout/MasterCardSection.vue'
import ProductCard from '@/components/sections/mycart/ProductCard.vue'
import TotalSection from '@/components/sections/mycart/TotalSection.vue'
import ButtonOrange from '@/components/elements/ButtonOrange.vue'
import Slider from '@/components/elements/Slider.vue'

defineProps({
    firstname: {
        type: String,
        default: 'fname'
    },

    lastname: {
        type: String,
        default: 'lname'
    },

    street: {
        type: String,
        default: 'street'
    },

    city: {
        type: String,
        default: 'city'
    },

    country: {
        type: String,
        default: 'country'
    },
    
})

</script>


<template>
    <div class="customerinfo-container">

        <div class="customerinfosection">
            <div class="customerinfo">
                <Separator/>
                <div class="customername">
                    <span class="name">
                        {{ firstname }} {{ lastname }}
                    </span>
                </div>
                <div class="address">
                    <span class="street">
                        {{ street }}
                    </span>
                    <span class="city">
                        {{ city }},
                    </span>
                    <span class="country">
                        {{ country }}
                    </span>
                </div>
                <Separator/>
            </div>
            <div class="arrow-container">
                    <button class="arrowbtn">
                        <img src="@/assets/images/svgs/checkoutarrow.svg" alt="" class="arrowicon">
                    </button>
            </div>
        </div>

            <MasterCardSection cardnum2="82"/>
            <div class="products">
                <ProductCard itemname="Nike React Miler" currency="$" price="170.00" class="product1"/>
                <ProductCard itemname="Nike Air Max 270" currency="$" price="112.00"/>
            </div>
            <TotalSection currency="$" price="282.00"/>
            <ButtonOrange link="/order" text="Place order" class="button" />
            <Slider class="slider"/>
    </div>
   
</template>


<style scoped>
.customerinfo-container{
    display: flex;
    width: 303px;
    margin-top: 47px;
    flex-direction: column;

}

.customerinfo{
    display: flex;
    flex-direction: column;

}
.customerinfosection{
    display: flex;
    
}


.customername{
    display: flex;
    width: 152px;
    margin-top: 14px;
    margin-bottom: 5px;


}
.address{
    display: flex;
    flex-direction: column;
    width: 187px;
    margin-bottom: 14px;
}
.name{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: 24px; /* 133.333% */
}

.street, .city, .country{
    color: #D5DDE0;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 500;
    line-height: 20px; /* 142.857% */
}

button{
    border: none;
    background: none;
    background-color:none;
    width: 11px;
    height: 10px;
    margin-left: -16px;
    cursor: pointer;
}

.arrow-container, .arrowbtn{
    display: flex;
    align-items: center;
    
}

.product1{
    margin-bottom: 16px;
}

.products{
    margin-top: 53px;
}

.button {
   margin-top: 27px;
}

.slider{
   
    margin-top: 670px;
}
</style>