<script setup>

defineProps({
    count: {
        type: String,
        default: 'currency'
    },

})
import MasterCardOrange from '@/components/sections/paymentmethod/MasterCardOrange.vue'
import MasterCardGrey from '@/components/sections/paymentmethod/MasterCardGrey.vue'
import CardDetailsForm from '@/components/sections/paymentmethod/CardDetailsForm.vue'
import ButtonOrange from '@/components/elements/ButtonOrange.vue'
import ButtonGrey from '@/components/elements/ButtonGrey.vue'
import OrSeparator from'@/components/sections/paymentmethod/OrSeparator.vue'


</script>


<template>
   <div class="paymentmethod-container">
        <div class="cards">
            <MasterCardOrange end="68" firstname="Luka" lastname="Marjanovic" month="09" year="22" class="orangecard"/>
            <MasterCardGrey end="68" firstname="Luka" lastname="Marjanovic" month="09" year="22" class="greycard" />
        </div>
        <CardDetailsForm/>
        <div class="btns">
            <ButtonOrange link="/addcard" text="Add card" class="button" />
            <OrSeparator text="Or"/>
            <ButtonGrey link="/scancard" text="Scan card" class="greybtn" />
        </div>
    </div>
</template>


<style scoped>

.paymentmethod-container{
    display: flex;
    width: 100%;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.cards{
    display: flex;
    width: 342px;
    overflow: hidden;
    justify-content: space-between;
    margin-left: 33px;
    margin-top: 47px;
}

.orangecard{
    margin-right: 16px;
}

.btns{
    margin-top: 42px;
}


</style>