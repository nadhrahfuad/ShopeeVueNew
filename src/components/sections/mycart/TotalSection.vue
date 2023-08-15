<script setup>

defineProps({
   
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

    <div class="total-container">
        <div class="totaltitle">
            <span class="intotal">
                In total
            </span>
        </div>
        <div class="totalprice">
            <span class="price">
                {{currency}} {{ price }}
            </span>
        </div>
    </div>

        
</template>

<style scoped>


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

</style>