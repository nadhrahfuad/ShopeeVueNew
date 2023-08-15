<script setup>
defineProps({
    cartnotifscount: {
        type: String,
        default: 'notifs'
    }
})

</script>


<template>
    <div class="cart-container">
        <div class="cartnotifs">
            <button class="cartbtn">
                <img src="@/assets/images/svgs/orangecart.svg" alt="" class="carticon">
            </button>
            <div class="notifs-container">
                <div class="circle">
                    <span class="number">
                        {{ cartnotifscount }}
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.cart-container{
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

.cartnotifs{
    display: flex;
    height: 34px;
    align-items: center;
    justify-content: center;
}

button{
    background-color: none;
    background: none;
    border: none;
    cursor: pointer;
}

.notifs-container{
    display: flex;
    position: absolute;
}

.circle{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 18px;
    height: 18px;
    border-radius: 50%;
    flex-shrink: 0;
    background-color: #FF5F00;
    border: #FFF 1px solid;
    margin-bottom: 27px;
    margin-right: 22px;

}
.number{
    color: #FFF;
    font-family: Roboto;
    font-size: 8px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}
</style>