<script setup>
import Separator from '@/components/elements/Separator.vue'
// @/assets/images/svgs/orangewalletpurchases.svg
</script>


<template>
    <div class="mypurchases-container">
        <div class="mypurchaseselements">
            <div class="purchasescardheader">
                <div class="title">
                    <span class="purchases">
                        My Purchases
                    </span>
                </div>
                <div class="purchasehistory">
                    <btn class="purchasehistorybtn">
                        <span class="purchasehistory">
                        View Purchase History
                        </span>
                        <span class="purchasehistoryarrow">
                        >
                        </span>
                    </btn>
                </div>
            </div>
            <Separator/>
            <div class="purchasesoptions">
                <div class="pay">
                    <button class="topay">
                        <img src="@/assets/images/svgs/topayicon.svg" alt="" class="topayicon">
                    </button>
                    <span class="paylabel">
                        To Pay
                    </span>
                </div>
                <div class="ship">
                    <button class="toship">
                        <img src="@/assets/images/svgs/toship.svg" alt="" class="shipicon">
                    </button>
                    <span class="label">
                        To Ship
                    </span>
                </div>
                <div class="receive">
                    <button class="toreceive">
                        <img src="@/assets/images/svgs/delivericon.svg" alt="" class="receiveicon">
                    </button>
                    <span class="label">
                        To Receive
                    </span>
                </div>
                <div class="rate">
                    <button class="torate">
                        <img src="@/assets/images/svgs/staricon.svg" alt="" class="staricon">
                    </button>
                    <span class="ratelabel">
                        To Rate
                    </span>
                </div>
                
            </div>
            <Separator/>
                <div class="purchasescardfooter">
                    <div class="title">
                        <span class="digital">
                            Digital Purchases
                        </span>
                    </div>
                    <div class="topup">
                        <btn class="viewtopupbtn">
                            <span class="viewtopup">
                            View my top-up
                            </span>
                            <span class="viewtopuparrow">
                            >
                            </span>
                        </btn>
                    </div>
                </div>
            

        </div>
    </div>
</template>

<style scoped>

.mypurchases-container{
    display: flex;
    width: 357px;
    height: 166px;
    flex-shrink: 0;
    border-radius: 19px;
    background: #FFF;
    justify-content: center;
    margin-top: 11px;
    box-shadow: -5px 15px 35px 0px rgba(35, 35, 35, 0.10);
}
.purchasescardheader{
    display: flex;
    width: 303px;
    justify-content: space-between;
    align-items: center;
    margin-top: 14px;
    margin-bottom: 8px;
}

.purchasescardfooter{
    display: flex;
    width: 303px;
    justify-content: space-between;
    align-items: center;
    margin-top: 4px;
}

button{
    background: none;
    border: none;
    background-color: none;
}
.purchasesoptions{
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 303px;
    justify-content: space-between;
    margin-top: 10px;
}

/* .rate.pay, */
.paylabel, .ratelabel{
    margin-top: 9px;
}

.rate, .pay{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
 .ship, .receive{
    display: flex;
    flex-direction: column;
    height: 47px;
    width: 47px;
    align-items: center;
    justify-content: center;
    
}

.shipicon, .receiveicon{
    display: flex;
    height: 47px;
    width: 47px;
}

.label, .paylabel, .ratelabel
{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-bottom: 21px;
}

.purchases, .digital{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.purchasehistory, .viewtopup{
    color: rgba(62, 73, 88, 0.48);
    font-family: Montserrat;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    cursor: pointer;
}

.purchasehistoryarrow, .viewtopuparrow{
    color: rgba(62, 73, 88, 0.48);
    font-family: MS Gothic;
    font-size: 8px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.toship, .toreceive, .torate, .topay{
    cursor: pointer;
}
</style>