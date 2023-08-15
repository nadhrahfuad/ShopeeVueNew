<script setup>
</script>


<template>
   <div class="codevoucher-container">
        <div class="voucherelements">
            <div class="codevoucher">
                <input type="text" class="voucher" placeholder="Enter code voucher">
            </div>
            <button class="applybutton">
                <span class="apply">
                    Apply
                </span>
            </button>
        </div>
  </div>
</template>


<style scoped>

.codevoucher-container{
    display: flex;
    width: 303px;
    /* 
    justify-content: flex-end; */
    
}
.codevoucher{
    display: flex;
    width: 189px;
    height: 60px;
    flex-shrink: 0;
    border-radius: 14px;
    border: 0.5px solid var(--grey, #D5DDE0);
    background: var(--grey-3, #F7F8F9);
    align-items: center;
    justify-content: center;
}
.applybutton{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 95px;
    height: 60px;
    flex-shrink: 0;
    border-radius: 14px;
    background: #D5DDE0;
}
.voucherelements{
    display: flex;
    width: 303px;
    align-items: center;
    justify-content: space-between;
    
}


input, button{
    border: none;
    background-color: none;
    background:none;
    outline: none; 
    
}

.apply{
    color: #FFF;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

::placeholder { 
    color: #D5DDE0;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}
</style>