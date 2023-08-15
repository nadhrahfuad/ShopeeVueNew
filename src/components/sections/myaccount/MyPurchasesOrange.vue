<script setup>
import Separator from '@/components/elements/Separator.vue'

defineProps({
    currency: {
        type: String,
        default: 'currency'
    },

    shopeepayprice: {
        type: String,
        default: 'price'
    },

    coin: {
        type: String,
        default: 'coin'
    },

    spaylaterprice: {
        type: String,
        default: 'spaylaterprice'
    },

    voucher:{
        type: String,
        default: 'voucher'
    }

})


</script>


<template>
    <div class="mypurchasesorange-container">
        <div class="mypurchasesorangeelements">
            <div class="purchasesorangecardheader">
                <div class="wallet-container">
                    <div class="walleticon">
                       <img src="@/assets/images/svgs/orangewalletpurchases.svg" alt="" class="walleticon">
                    </div>
                </div>
                <div class="title">
                    <span class="purchases">
                        My Purchases
                    </span>
                </div>
            </div>
            <Separator/>
            <div class="orangepurchasesoptions">
                <div class="shopeepay">
                    <button class="shopeepaybtn">
                        <img src="@/assets/images/svgs/shopeewalleticon.svg" alt="" class="shopeepayicon">
                        <span class="innerSshopee">S</span>
                    </button>
                    <span class="label">
                        Shopee Pay
                    </span>
                    <span class="price">
                        {{ currency }} {{ shopeepayprice }}
                    </span>
                </div>
                <div class="coin">
                    <button class="coinbtn">
                        <span class="innerS">S</span>
                    </button>
                    <span class="label">
                        Shopee Coins
                    </span>
                    <span class="price">
                        {{ coin }} Koin
                    </span>
                    
                </div>
                <div class="spaylater">
                    <button class="spaylaterbtn">
                        <img src="@/assets/images/svgs/cardicon.svg" alt="" class="receiveicon">
                    </button>
                    <span class="label">
                        SPayLater
                    </span>
                    <span class="price">
                        {{ currency }} {{ spaylaterprice }}
                    </span>
                </div>
                <div class="voucher">
                    <button class="voucherbtn">
                        <img src="@/assets/images/svgs/vouchericon.svg" alt="" class="vouchericon">
                    </button>
                    <span class="label">
                        My Voucher
                    </span>
                    <span class="price">
                        {{ voucher }} Voucher
                    </span>
                </div>
                
            </div>

        </div>
    </div>
</template>

<style scoped>
.mypurchasesorange-container{
    display: flex;
    width: 357px;
    height: 147px;
    flex-shrink: 0;
    border-radius: 19px;
    background: #FFF;
    justify-content: center;
    margin-top: 8px;
    box-shadow: -5px 15px 35px 0px rgba(35, 35, 35, 0.10);
}
.purchasesorangecardheader{
    display: flex;
    width: 303px;
    height: 18px;
    align-items: center;
    margin-top: 14px;
    margin-bottom: 8px;
}

.price{
    color: #FF5F00;
    text-align: center;
    font-family: Montserrat;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

button{
    background: none;
    border: none;
    background-color: none;
}
.orangepurchasesoptions{
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 303px;
    justify-content: space-between;
    margin-top: 33px;
}

.voucher, .shopeepay{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
 .coin, .spaylater{
    display: flex;
    flex-direction: column;
    height: 47px;
    width: 47px;
    align-items: center;
    justify-content: center;
    
}

.shopeepayicon{
    margin-bottom: 8px;
}
 .cardicon{
    display: flex;
    width: 38px;
    height: 38px;
}

.purchases{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-left: 8px;
}

.wallet-container{
    color: rgba(62, 73, 88, 0.48);
    font-family: Montserrat;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    cursor: pointer;
}


.label{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.coinbtn, .spaylaterbtn, .voucherbtn, .shopeepaybtn{
    cursor: pointer;
}

.coinbtn{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 31px;
    height: 31px;
    border-radius: 50%;
    border: 2.5px solid #FF5F00;
    margin-bottom: 6px;
}

.innerS{
    width: 6px;
    height: 12px;
    flex-shrink: 0;
    color: #FF5F00;
    font-family: Roboto;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.innerSshopee{
    position: absolute;
    width: 6px;
    height: 12px;
    flex-shrink: 0;
    color: #FF5F00;
    font-family: Roboto;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-top: 10px;
    margin-left: -17px;
}

.shopeepay, .coin, .spaylater, .voucher{
    display:flex;
    align-items: center;
    justify-content: center;
    width: 55px;
    height: 63px;

}

</style>