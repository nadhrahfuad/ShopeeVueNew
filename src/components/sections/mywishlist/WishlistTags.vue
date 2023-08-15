<script setup>
defineProps({
    sale: {
        type: String,
        default: 'sale'
    },
    picnum: {
        type: String,
        default: '0/10'
    }
})

</script>


<template>
    <div class="wishlisttags-container">
        <div class="wishlistelements">
            <div class="saletag-container">
                <div class="saletag">
                    <span class="sale">
                        {{ sale }}
                    </span>
                </div>
            </div>
            <div class="deliver-container">
                <div class="delivertag">
                    <img src="@/assets/images/svgs/truckicon.svg" alt="" class="truckicon">
                    <span class="deliver">
                        GRATIS ONGKIR
                    </span>
                </div>
            </div>
            <div class="cashback-container">
                <div class="cashbacktag">
                    <span class="cashback">
                        CASHBACK
                    </span>
                </div>
            </div>   
        </div>
        <div class="picselection-container">
            <div class="picselection">
                <span class="picnum">
                    {{ picnum }}
                </span>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wishlisttags-container{
    display: flex;
    width: 357px;
    align-items: center;
    justify-content: space-between;
    margin-top:195px;
    /* margin-bottom:6px; */
}

.wishlistelements{
    display: flex;
    flex-direction:row;
    width: 83px;
    justify-content: space-between
}

.saletag{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 26px;
    height: 8px;
    border-radius: 4px;
    background: #FF5F00;
}

.delivertag{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 25px;
    height: 8px;
    flex-shrink: 0;
    border-radius: 4px;
    background: #1152FD;
}

.cashbacktag{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 30px;
    height: 8px;
    flex-shrink: 0;
    border-radius: 4px;
    background: #B4B4B4;
}

.picselection{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 46px;
    height: 14px;
    border-radius: 7px;
    background: rgba(180, 180, 180, 0.45);

}

.sale{
    color: #FFF;
    font-family: Montserrat;
    font-size: 5px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
}

.deliver{
    width:9px;
    color: #FFF;
    font-family: Montserrat;
    font-size: 2px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
}

.cashback{
    color: #FFF;
    font-family: Montserrat;
    font-size: 4px;
    font-style: normal;
    font-weight: 800;
    line-height: normal;
}

.picnum{
    color: #000;
    font-family: Montserrat;
    font-size: 10px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
</style>