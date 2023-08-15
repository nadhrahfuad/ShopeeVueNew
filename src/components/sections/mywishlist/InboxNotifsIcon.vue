<script setup>
defineProps({
    inboxnotifscount: {
        type: String,
        default: 'notifs'
    }
})

</script>


<template>
    <div class="inbox-container">
        <div class="inboxnotifs">
            <button class="inboxicon-container">
                <img src="@/assets/images/svgs/orangeinbox.svg" alt="" class="inboxicon">
            </button>
            <div class="notifs-container">
                <div class="circle">
                    <span class="number">
                        {{ inboxnotifscount }}+
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

.inbox-container{
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

.inboxnotifs{
    display: flex;
    height: 34px;
    align-items: center;
    justify-content: center;
}

button{
    background-color: none;
    background: none;
    border: none;
    cursor: pointer;
}

.notifs-container{
    display: flex;
    position: absolute;    
    
}

.circle{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 18px;
    height: 18px;
    border-radius: 50%;
    background-color: #FF5F00;
    border: #FFF 1px solid;
    margin-bottom: 27px;
    margin-right: 22px;

    
}
.number{
    color: #FFF;
    font-family: Roboto;
    font-size: 8px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}
</style>