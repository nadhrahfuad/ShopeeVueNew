<script setup>

defineProps({
  
    link: {
        type: String,
        default: '/'
    }
})

</script>


<template>
    <a class="camerabutton" :href="link"> 
        <img src="@/assets/images/svgs/camicon.svg" alt="" class="cameraicon">
    </a>
</template>


<style scoped>
a {
    display: flex;
    justify-content: center;
    align-items: center;
}

.camerabutton {
    width: 60px;
    height: 60px;
    flex-shrink: 0;
    border-radius: 14px;
    background: #D5DDE0;
}
</style>