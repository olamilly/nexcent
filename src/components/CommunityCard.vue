<template>
    <div class="containery">
        <component :is="content.logo"></component>
         <h2>{{ content.header }}</h2>
         <p>{{ content.description }}</p>
    </div>
</template>
<script setup lang="ts">
import { ref } from "vue";
import MembershipLogo from "../assets/MembershipLogo.vue";
import NationalLogo from "../assets/NationalLogo.vue";
import ClubsLogo from "../assets/ClubsLogo.vue";
const props = defineProps({box:{
    type:String,
    Required: true
}})

const content =ref({
    logo:ClubsLogo,
    header:'',
    description:'Our membership management software provides full automation of membership renewals and payments.'
})

if(props.box == "membership"){
    content.value.logo= MembershipLogo
    content.value.header= "Membership Organizations"
}
else if(props.box == "national"){
    content.value.logo= NationalLogo
    content.value.header= "National Associations"
}
else{
    content.value.logo= ClubsLogo
    content.value.header="Clubs and Groups"
}
</script>
<style scoped>
.containery{
    padding: 1rem;
    box-shadow: 3px 3px #f8f7f7;
    border-radius: 3px;
    min-height: 242px;
    margin-bottom: .6rem;
    transition : 0.3s ease-in-out;
}
.containery:hover{
    transform: scale(1.2,1.2);
    
}
h2{
    color: #4D4D4D;
    margin-top:.2rem;
    font-size: 1.3rem;
}
p{
    color:#717171;
    font-size: .7rem;
}
</style>