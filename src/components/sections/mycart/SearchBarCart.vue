<script setup>
</script>


<template>
   <div class="searchbar-container">
        <div class="searchbar">
            <div class="searchbarleftelements">
                <div class="searchicon-container">
                    <img src="@/assets/images/svgs/searchicon.svg" alt="" class="searchicon">
                </div>
                <div class="searchinput">
                    <input type="text" class="search" placeholder="Search">   
                </div>
            </div>
            <!-- <div class="searchbarrightelements">
                <button class="camerabtn">
                    <img src="@/assets/images/svgs/cameraicon.svg" alt="" class="cameraicon">
                </button>
            </div> -->
        </div>
   
  </div>
</template>


<style scoped>

.searchbar-container{
    display: flex;
    /* width: 303px;
    justify-content: flex-end; */
    
}
.searchbar{
    display: flex;
    width: 303px;
    height: 60px;
    flex-shrink: 0;
    border-radius: 14px;
    border: 0.5px solid var(--grey, #D5DDE0);
    background: var(--grey-3, #F7F8F9);
    /* justify-content: space-evenly; */
}

.searchbarleftelements{
    display: flex;
    align-items: center;
    
}

.searchicon-container{
    display: flex;
    width: 19.707px;
    height: 19.707px;
    flex-shrink: 0;
    fill: #D5DDE0;
    cursor: pointer;
    margin-left: 18px;
}
input, button{
    border: none;
    background-color: none;
    background:none;
    outline: none; 
    
}

::placeholder { 
    color: #D5DDE0;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}

.camerabtn{
    display: flex;
    cursor: pointer;
    
}
</style>