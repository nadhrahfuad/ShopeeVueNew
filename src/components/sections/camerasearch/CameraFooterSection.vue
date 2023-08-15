<template>
    <div class="CameraFooterContainer">

        <div class="footerelements">
            <div class="title">
                <span class="connectdots">
                    Move your camera to connect the dots
                </span>
            </div>
            <div class="footeroptionscontainer">
                <div class="footeroptions">
                    <div class="pictureselect">
                        <button class="gallery">
                            <img src="@/assets/images/pictures/gallerybtnpic.png" alt="" class="gallerypic">
                        </button>
                    </div>
                    <div class="camerabtn">
                        <button class="camera">
                            <div class="outer">
                                <div class="inner">

                                </div>
                            </div>
                        </button>
                    </div>
                    <div class="flipbtn">
                        <button class="flip">
                            <img src="@/assets/images/svgs/flip.svg" alt="" class="flipicon">
                        </button>
                    </div>
                </div>
            </div>
        </div>
       
    </div>
    <Slider/>
    
</template>

<script setup>
import Slider from '@/components/elements/Slider.vue'
</script>

<style scoped>
.CameraFooterContainer {
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    margin-top: -131px;
    width: 100%;
    
   
}

.footerelements{
    display:flex;
    width: 100%;
    justify-content:center;
    align-items:center;
    flex-direction: column;
}
.title{
    display:flex;
    margin-bottom: 31px;
}
.connectdots{
    display:flex;
    color: #97ADB6;
    font-family: Montserrat;
    font-size: 12px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;

}

.footeroptionscontainer{
    display: flex;
    flex-direction: row;
    height: 64px;
    align-items:center;
    width: 100%;
    justify-content: center;
}

.footeroptions{
    display: flex;
    height: 64px;
    align-items:center;
    width: 100%;
    justify-content: space-around;
}

button{
    border: none;
    background:none;
    display: flex;
}

.gallery{
    display:flex;
    width: 49px;
    height: 49px;
    border-radius: 8px;
    background: rgba(17, 82, 253, 0.25);
    justify-content:center;
    align-items: center;
}

.pictureselect{
    display: flex;
    width: 64px;
    justify-content: center;

}

.gallerypic{
    display:flex;
    width: 49px;
    height: 49px;
    border-radius: 8px;

}

.camerabtn{
    display:flex;
    width: 64px;
    height: 64px;
    justify-content: center;
}

.outer{
    display:flex;
    width: 64px;
    height: 64px;
    border-radius: 50%;
    border: #97ADB6 solid 3px;
    justify-content:center;
    align-items: center;
}

.inner{
    display:flex;
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background-color: #FF5F00;
}

.flipbtn{
    display:flex;
    width: 64px;
    height: 20px;
    justify-content: center;

}





</style>