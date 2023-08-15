<script setup>
import InboxNotifsIcon from '@/components/sections/mywishlist/InboxNotifsIcon.vue'
import CartNotifsIcon from '@/components/sections/mywishlist/CartNotifsIcon.vue'


</script>


<template>
    <div class="wishlistheader-container">
        <div class="headerelements">
            <div class="orangearrowcontainer">
                <img src="@/assets/images/svgs/orangearrow.svg" class="orangearrowicon" alt="Go Back" @click="$router.go(-1)">
            </div>
            <div class="notifications">
                <div class="cart">
                    <CartNotifsIcon cartnotifscount="12"/>
                </div>
                <div class="inbox">
                    <InboxNotifsIcon inboxnotifscount="99"/>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wishlistheader-container{
    display: flex;
    flex-direction: row;
    margin-top:33px;
    
}
.headerelements{
    display: flex;
    width: 357px;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}
.notifications{
    display: flex;
    flex-direction: row;
    align-items: center
}

.orangearrowicon{
    cursor: pointer;
}
</style>