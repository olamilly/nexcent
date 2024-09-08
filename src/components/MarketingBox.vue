<template>
    <div class="containery">
        <component v-if="props.box=='one'" :is="FillerImage1"></component>
        <component v-if="props.box=='two'" :is="FillerImage2"></component>
        <component v-if="props.box=='three'" :is="FillerImage3"></component>
        <div class="outer-box">
            <div class="text-box">
                <h4>{{ content.description }}</h4>
                <a>
                    Read More
                    <svg width="18" height="21" viewBox="0 0 6 7" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M4.42153 4.5177L5.24609 3.69314C5.34388 3.59535 5.34388 3.4368 5.24609 3.33901L4.42153 2.51445M5.17274 3.51607L1.50012 3.51607" stroke="#4CAF4F" stroke-width="0.367253" stroke-linecap="round"/>
                    </svg>
                </a>
            </div>
        </div>
        
    </div>
</template>
<script setup lang="ts">
import FillerImage1 from '@/assets/FillerImage1.vue';
import FillerImage2 from '@/assets/FillerImage2.vue';
import FillerImage3 from '@/assets/FillerImage3.vue';
import { ref } from "vue";
const props = defineProps({box:{
    type:String,
    Required: true
}})

const content =ref({
    description:'Our membership management software provides full automation of membership renewals and payments.'
})

if(props.box == "one"){
    // content.value.img= FillerImage1
    content.value.description= "Creating Streamlined Safeguarding processes with OneRen"
}
else if(props.box == "two"){
    // content.value.img= FillerImage3
    content.value.description="What are your safeguarding responsibilities and how can you manage them"
}
else{
    // content.value.img= FillerImage2
    content.value.description= "Revamping the Membership Model with Triathlon Australia"
}

</script>
<style scoped>
.containery{
    position: relative;
}
.text-box{
    width: 85%;
    
    background-color: #F5F7FA;
    border-radius: 5px;
    padding-top: .8rem;
    padding-bottom: .8rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 105px;
}
.outer-box{
    display: flex;
    justify-content: center;
    position: absolute;
    top:65%;
}
@media(max-width: 767.98px){
    .outer-box{
    width: 100%;
    
}
.text-box{
    width: 55%;
    max-width:200px;
}

}
a{
    color:#4CAF4F !important;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: .6rem;
}
h4{
    font-size:.8rem;
    color: #4D4D4D;
}
</style>