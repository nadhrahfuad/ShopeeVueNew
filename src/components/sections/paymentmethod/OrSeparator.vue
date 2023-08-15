<script setup>

defineProps({
    text: {
        type: String,
        default: 'Sign/Up with'
    }

})

</script>

<template>
    <div class="separator-container">
        <div class=method-container>
            <img src="@/assets/images/shapes/Rectangle57.svg" alt="------------">
            <span>{{ text }}</span>
            <img src="@/assets/images/shapes/Rectangle57.svg" alt="------------">
        </div>
    </div>
</template>

<style scoped>
.separator-container {
    margin-top: 22px;
    width: 303px;
    margin-bottom: 21px;
    /* background-color: rgb(160, 160, 160); */
}

.method-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.method-container>span {
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

img{
    width: 132px;
}


</style>
