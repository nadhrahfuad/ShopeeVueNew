<script setup>

defineProps({
    end: {
        type: String,
        default: 'Card end'
    },

    firstname: {
        type: String,
        default: 'fname'
    },

    lastname: {
        type: String,
        default: 'lname'
    },

    month: {
        type: String,
        default: 'month'
    },

    year: {
        type: String,
        default: 'year'
    }
})

</script>
<!--  -->

<template>
   <div class="card-container">
        <div class="card">
            <div class="cardelements">
                <div class="mclogo">
                    <img src="@/assets/images/svgs/masctercardlogo.svg" alt="" class="mastercardlogo">
                </div>
                <div class="orangechip">
                    <img src="@/assets/images/svgs/greychip.svg" alt="" class="cardchipicon">
                </div>
                <div class="cardnumber-container">
                    <span class="cardnumber">
                        **** **** **** **{{ end }}
                    </span>
                </div>
                <div class="cardinfo">
                    <div class="details-container">
                        <div class="name">
                            <span class="cardname">
                                {{ firstname }} {{ lastname }}
                            </span>
                        </div>
                        <div class="expiry">
                            <span class="cardexpiry">
                                {{ month }}/{{ year }}
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
       
</template>


<style scoped>

.card{
    display: flex;
    flex-direction: column;
    width: 260px;
    height: 154px;
    flex-shrink: 0;
    border-radius: 16px;
    background: linear-gradient(90deg, #4A5562 0%, #FFF 100%, #FF985A 100%);
    backdrop-filter: blur(115px);
}

.cardelements{
    display: flex;
    flex-direction: column;
    margin-left: 17px;
    margin-right: 21px;
    margin-top: 20px;
}

.cardchipicon{
    display: flex;
    justify-content: flex-start;
    margin-bottom: 2px;
}

.mclogo{
    display: flex;
    justify-content: flex-end;
}

.details-container{
    display: flex;
    width: 100%;
    flex-direction: row;
    justify-content: space-between;
}

.cardnumber{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    letter-spacing: 2.8px;
    margin-left: 5px;
    margin-bottom: 22px;
}

.cardname{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 11px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-left: 5px;
}

.cardexpiry{
    color: #3E4958;
    font-family: Montserrat;
    font-size: 11px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
</style>