<script setup>

defineProps({
    count: {
        type: String,
        default: 'currency'
    },

    product: {
        type: String,
        default: 'product'
    },
    
    rating: {
        type: String,
        default: 'rating'
    },

    chat: {
        type: String,
        default: 'chat'
    },
})

</script>


<template>
   <div class="productrating-container">
        <div class="product">
            <div class="num-container">
                <span class="num">
                    {{ product }}
                </span>
                <span class="count">
                    {{ count }}
                </span>
            </div>
            <div class="label-container">
                <span class="label">
                    Product
                </span>
            </div>
        </div>
        <div class="rating">
            <div class="num-container">
                <span class="num">
                    {{ rating }}
                </span>
            </div>
            <div class="label-container">
                <span class="label">
                    Rating
                </span>
            </div>
        </div>
        <div class="chat">
            <div class="num-container">
                <span class="num">
                    {{ chat }}%
                </span>
            </div>
            <div class="label-container">
                <span class="label">
                    Chat
                </span>
            </div>
            
        </div>
    </div>
</template>


<style scoped>

.productrating-container{
    display: flex;
    width: 357px;
    justify-content: space-evenly;
    margin-top: 2px;
}
.num-container, .label-container{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 55px;
}
.num, .count{
    color: #EB001B;
    text-align: center;
    font-family: Montserrat;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.label{
    width: 55px;
    color: #1F1F1F;
    text-align: center;
    font-family: Montserrat;
    font-size: 10px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
}


</style>