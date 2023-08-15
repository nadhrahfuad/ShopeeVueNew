<script setup>

</script>


<template>
   <div class="variation-container">
        <div class="variationelements">
            <div class="variationlabel">
                <div class="variationtitle">
                    <span class="title">
                        Pilih Variasi
                    </span>
                </div>
                <div class="variationsuntitle">
                    <span class="subtitle">
                        &nbsp;(Warna, Ukuran)
                    </span>
                </div>
            </div>
            <div class="arrowbtn">
                <button class="arrowicon">
                    <span class="arrow">
                        >
                    </span>
                </button>
            </div>
            
        </div>
    </div>
</template>


<style scoped>

.variation-container{
    display: flex;
    width: 357px;
    height: 28px;
    flex-shrink: 0;
    background-color: #FFF;
    border-radius: 19px;
    box-shadow: -5px 15px 35px 0px rgba(35, 35, 35, 0.10);
    align-items: center;
    justify-content: center;
    margin-top: 11px;
}

.variationelements{
    display: flex;
    width: 326px;
    justify-content: space-between;
}

.variationlabel{
    display: flex;
    width: 200px;
}

.arrowicon{
    cursor: pointer;
}

button{
    border: none;
    background-color: none;
    background: none;
}
.title{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.subtitle{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 9px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.arrow{
    width: 12px;
    color: #3E4958;
    font-family: MS Gothic;
    font-size: 11px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

</style>