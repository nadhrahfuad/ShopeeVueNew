<template>
    <div class="DialContainer">

        <div class="dash">
            <div class="ellipse"></div>
        </div>
       
    </div>
</template>

<script setup>
</script>

<style scoped>
.DialContainer {
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    margin-top: 550px;
    width:100%;
    height:155px;
    
    
   
}

.dash{
    display:flex;
    width: 550px;
    height: 461px;
    flex-shrink: 0;
    border-radius: 50%;
    border: 2px dashed #FFF;
    justify-content:center;
    
    
   
}

.ellipse{
    display:flex;
    flex-direction: column;
    width: 12px;
    height: 12px;
    border-radius:50%;
    background-color:white;
    margin-top: -7.5px;
    
    

}
</style>