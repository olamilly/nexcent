<template>
    <div class="containery">
        <header>
            <h1 class="section-title">Our Clients</h1>
            <p class="description">We have been working with some Fortune 500 clients</p>
        </header>
        <div class="client-logos">
            <div class="brand-group"><component v-for="brand, index in brandsGroup1" :key="index" :is="brand"></component></div>
            <div class="brand-group"><component v-for="brand, index in brandsGroup2" :key="index" :is="brand"></component></div>
        </div>
    </div>
</template>
<style scoped>
.containery{
    margin-top:3.5rem;
}
.client-logos{
    display: flex;
    width: 100%;
    align-items: center;
    margin-bottom:3.5rem;
}
.brand-group{
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 100%;
}
@media(max-width: 767.98px) {
    .client-logos{
        flex-direction: column;
    }
    .brand-group{
        width: 60%;
    }
}
</style>
<script setup lang="ts">
import Brand3Logo from "@/assets/brand3Logo.vue";
import Brand1Logo from "@/assets/brand1Logo.vue";
import Brand2Logo from "@/assets/brand2Logo.vue";
import Brand4Logo from "@/assets/brand4Logo.vue";
import Brand5Logo from "@/assets/brand5Logo.vue";
import Brand6Logo from "@/assets/brand6Logo.vue";

const brandsGroup1:Array<any> =[Brand1Logo, Brand2Logo, Brand3Logo]
const brandsGroup2:Array<any> =[Brand4Logo, Brand5Logo, Brand6Logo]
</script>