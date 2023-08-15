<!--  -->

<script setup>

import Separator from '@/components/elements/Separator.vue'

defineProps({
    cardnum2: {
        type: String,
        default: 'endnum'
    },
    
})

</script>


<template>
    <div class="mastercard-container">

        <div class="carddetailselements">
            <div class="leftelements">
                <div class="logo">
                    <img src="@/assets/images/svgs/mastercard.svg" alt="" class="mastercardlogo">
                </div>
                <div class="carddetails">
                    <span class="cardendnum">
                        Master Card ending **{{cardnum2}}
                    </span>
                </div>
            </div>
            <div class="arrow-container">
                    <button class="arrowbtn">
                        <img src="@/assets/images/svgs/checkoutarrow.svg" alt="" class="arrowicon">
                    </button>
            </div>
        </div>

        <Separator/>
    </div>
</template>


<style scoped>
.mastercard-container{
    display: flex;
    width: 303px;
    margin-top: 20px; 
    flex-direction: column;
    
}

.leftelements{
    display: flex;
    align-items: center;
}

.logo{
    margin-right: 10px
}

.carddetailselements{
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-bottom: 12.62px;
    justify-content: space-between
}
.cardendnum{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

button{
    border: none;
    background: none;
    background-color:none;
    width: 11px;
    height: 10px;
    cursor: pointer;
}

.arrow-container, .arrowbtn{
    display: flex;
    align-items: center;
    
}
</style>