<script setup>
defineProps({
    currency: {
        type: String,
        default: 'currency'
    },

    redeemprice: {
        type: String,
        default: 'redeem'
    },

    off: {
        type: String,
        default: 'off'
    },

    spaylaterprice: {
        type: String,
        default: 'spaylaterprice'
    }
})
</script>


<template>
   <div class="voucher-container">
        <div class="voucherelements">
            <div class="redeem">

                <div class="label">
                    <span class="redeemlabel">
                        Ongkos Kirim
                    </span>
                </div>

                <div class="price">
                    <div class="redeemprice">
                        <span class="currency">
                            {{ currency }}
                        </span>
                        <span class="redeemprice">
                            {{ redeemprice }}
                        </span>
                    </div>
                </div>
            </div>

            <div class="claim">
                <div class="label">
                    <span class="claimlabel">
                        Claim Voucher
                    </span>
                </div>
                <div class="price">
                    <div class="off-container">
                        <span class="off">
                            {{ off }}% OFF
                        </span>
                    </div>
                </div>
            </div>

            <div class="spaylater">
                <div class="label">
                    <span class="spaylaterlabel">
                        SPayLater
                    </span>
                </div>
                <div class="price">
                    <div class="spaylaterprice">
                        <span class="currency">
                                {{ currency }}
                        </span>
                        <span class="paylaterprice">
                            {{ spaylaterprice }}>
                        </span>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>


<style scoped>

.voucherelements{
    display: flex;
    flex-direction: column;
    width: 333px;
    
}
.redeem, .claim, .spaylater{
    display: flex;
    flex-direction: row;
    width: 100%;
    justify-content: space-between;
    margin-top: 7px;;
}

.price, .spaylaterprice{
    display: flex;
    align-items: center;
}

.spaylater{
    display: flex;
    margin-bottom: 17px;
}

.price{
    cursor: pointer;
}
.redeemlabel, .claimlabel, .spaylaterlabel{
    width: 120px;
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.currency, .redeemprice, .paylaterprice{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 11px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.off-container{
    display: flex;
    width: 86px;
    height: 17px;
    flex-shrink: 0;
    border-radius: 2px;
    background: #FF5F00;
}
.off{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    color: #FFF;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
</style>