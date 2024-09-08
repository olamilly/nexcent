<template>
    <div class="containery">
        <header>
            <h1 class="section-title">Caring is the new marketing</h1>
            <p class="description">The Nextcent blog is the best place to read about the latest membership insights, trends and more. See who's joining the community, read about how our community are increasing their membership income and lot's more.</p>
        </header>
        <div v-if="screen<=767" id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
            
        <div class="carousel-inner">
            <div class="carousel-item active">
                <box box="one" />
            </div>
            <div class="carousel-item">
                <box box="two" />
            </div>
            <div class="carousel-item">
                <box box="three" />
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="false"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="false"></span>
            <span class="visually-hidden">Next</span>
        </button>
        </div>
        <div class="links" v-if="screen>767">
            <box box="one" />
            <box box="two" />
            <box box="three" />
        </div>
    </div>
</template>
<style scoped>
h1{
    margin-bottom: 8px;
}
@media(max-width: 767.98px){

p.description{
    width: 100%;
}
}
.containery{
    margin-bottom: 3rem;
}
.description{
    width:55%;
}
.links{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
span.carousel-control-prev-icon, span.carousel-control-next-icon{
   background-color: #A5D6A7;
   border-radius: 4px;
}


</style>
<script setup lang="ts">

import { markRaw, onMounted, ref } from 'vue';
import MarketingBox from './MarketingBox.vue';
const box =markRaw(MarketingBox)
const screen=ref(window.screen.width)
onMounted(()=>{
    window.addEventListener('resize', function() { 
        screen.value=window.screen.width
    })
    
})
</script>