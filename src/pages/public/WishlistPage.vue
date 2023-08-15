<script setup>
import WhiteContainer from '@/components/container/WhiteContainer.vue';
import WishlistHeader from '@/components/sections/mywishlist/WishlistHeader.vue';
import BottomNavigation from "@/components/navigations/BottomNavigation.vue";
import WishlistTags from '@/components/sections/mywishlist/WishlistTags.vue'
import ItemCard from '@/components/content/ItemCardWishlistContent.vue'
import VariationCardWishlistContent from '@/components/content/VariationCardWishlistContent.vue';
import VoucherContentWishlist from '@/components/content/VoucherContentWishlist.vue';
import StoreCardWishlist from '@/components/content/StoreCardWishlist.vue'
</script>

<template>
    <div class="back">
        <WhiteContainer class="bg">
            <WishlistHeader/>
            <WishlistTags sale="12.12" picnum="1/10"/>
            <ItemCard itemname="Erigo Coach Jacket Apparel Tokyo Nevy" currency="Rp." price="149.000" oldprice="199.000" sold="1,7RB"/>
            <VariationCardWishlistContent/>
            <VoucherContentWishlist currency="Rp." redeemprice="0" off="50" spaylaterprice="10.62.912"/>
            <StoreCardWishlist storename="ErigoStore" location="DKI Jakarta" active="16"/>
            <BottomNavigation/>
        </WhiteContainer>
    </div>
</template>

<style scoped>
.bg{
    /* width: 375px; */
    height: 308px;
    background-color: white;
    -webkit-border-radius: 20px;
    -moz-border-radius: 20px;
    border-radius: 20px;
    background-image: url('@/assets/images/pictures/wishlistbg.png');
    background-repeat: no-repeat;
    border-radius: 20px;
    
    /* margin: 20px; */
}

.back{
    width: 375px;
    height: 812px;
    background-color: #FFF;
    border-radius: 20px;
}
</style>

