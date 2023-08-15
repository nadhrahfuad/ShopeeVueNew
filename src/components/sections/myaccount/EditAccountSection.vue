<script setup>
import EditAccountButton from '@/components/sections/myaccount/EditAccountButton.vue'
// import ProductCard from '@/components/sections/mycart/ProductCard.vue'
// import SearchBarCart from '@/components/sections/mycart/SearchBarCart.vue'
// import CodeVoucherSection from '@/components/sections/mycart/CodeVoucherSection.vue'
// import TotalSection from '@/components/sections/mycart/TotalSection.vue'

defineProps({
    firstname: {
        type: String,
        default: 'fname'
    },

    lastname: {
        type: String,
        default: 'lname'
    }

})


</script>


<template>
    <div class="editaccount-container">
        <div class="editaccount">
            <div class="accountpfp">
                <img src="@/assets/images/pictures/accountpfp.png" alt="" class="pfp">
            </div>
            <div class="name-container">
                <div class="accountname">
                    <span class="name">{{ firstname }} {{ lastname }}</span>
                </div>
                <EditAccountButton text="Edit account"/>
            </div>
            

        </div>
    </div>
</template>

<style scoped>
.editaccount{
    display:flex;
    align-items: center;
    /* justify-content: center; */
    margin-top: 47px;
    margin-left: 27px;
}

.name-container{
    display: flex;
    flex-direction: column;
    margin-left: 18px;
}

.accountname{
    margin-bottom: 11px;
}
.accountpfp, .pfp{

    width: 77px;
    height: 77px;
    flex-shrink: 0;
    border-radius: 14px;
    background: var(--grey-3, #F7F8F9);

}

.name{

    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;

}



</style>