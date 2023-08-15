<script setup>

defineProps({
    text: {
        type: String,
        default: 'Title of Button Here'
    },

    link: {
        type: String,
        default: '/'
    }
})

</script>


<template>
    <a class="button" :href="link"> {{ text }} </a>
</template>


<style scoped>
a {
    display: flex;
    justify-content: center;
    align-items: center;
    color: #D5DDE0;
    font-family: Montserrat;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    }

.button {
    width: 101px;
    height: 36px;
    flex-shrink: 0;
    border-radius: 7px;
    border: 0.5px solid #D5DDE0;
    background: #F7F8F9;
}
</style>