<script setup>

defineProps({
    end: {
        type: String,
        default: 'Card end'
    },

    firstname: {
        type: String,
        default: 'fname'
    },

    lastname: {
        type: String,
        default: 'lname'
    },

    month: {
        type: String,
        default: 'month'
    },

    year: {
        type: String,
        default: 'year'
    }
})

import Separator from '../../elements/Separator.vue';

</script>
<!--  -->

<template>
   <div class="carddetailsform-container">
        <div class="formelements">
            <div class="cardnumber">
                <input type="text" name="" value="" placeholder="Card number">
                <Separator/>
            </div>
            <div class="cardholdername">
                <input type="text" name="" value="" placeholder="Card holder name">
                <Separator/>
            </div>
            <div class="expirynsecurity">
                <div class="expiry">
                    <input type="text" name="" value="" placeholder="Expiry date">
                    <div class="short"></div>
                </div>
                <div class="security">
                    <input type="text" name="" value="" placeholder="Security code">
                    <div class="short"></div>
                </div>
            </div>
            <div class="cvv">
                <input type="text" name="" value="" placeholder="CVV">
                <Separator/>
            </div>
            
        </div>
    </div>
       
</template>


<style scoped>
.carddetailsform-container{
    display: flex;
    width: 100%;
    justify-content: center;
    margin-top: 50px;
}

.formelements{
    display: flex;
    width: 303px;
    flex-direction: column;
}

input{
    border: none;
    background: none;
    margin-bottom: 8px;
}

.expirynsecurity{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 33px;
}

.short{
    width: 142px;
    height: 1px;
    flex-shrink: 0;
    background: #D5DDE0;
}

::placeholder { 
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.cvv, .cardholdername{
    margin-top: 33px;
}

</style>