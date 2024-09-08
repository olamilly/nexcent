<template>
    <div class="containery">
        <div class="illustration">
            <PanaIllustration />
        </div>
        <div class="frame6-container">
            <div class="frame6">
                <h2>How to design your site footer like we did</h2>
                <p>Donec a eros justo. Fusce egestas tristique ultrices. Nam tempor, augue nec tincidunt molestie, massa nunc varius arcu, at scelerisque elit erat a magna. Donec quis erat at libero ultrices mollis. In hac habitasse platea dictumst. Vivamus vehicula leo dui, at porta nisi facilisis finibus. In euismod augue vitae nisi ultricies, non aliquet urna tincidunt. Integer in nisi eget nulla commodo faucibus efficitur quis massa. Praesent felis est, finibus et nisi ac, hendrerit venenatis libero. Donec consectetur faucibus ipsum id gravida.</p>
                <button class="medium">Learn More</button>
            </div>
        </div>
        
    </div>
</template>
<script setup lang="ts">
import PanaIllustration from '@/assets/panaIllustration.vue';

</script>
<style scoped>
.containery{
    display: flex;
    align-items: center;
    margin-bottom: 2rem;
}
@media (max-width: 767.98px) {
    .containery{
        flex-direction: column;
    }
    .illustration, .frame6-container,.frame6{
        width:100%;
    }
    .frame6{
        text-align: center;
    }
    .frame6-container{
        justify-content: center;
    }
}
.illustration{
    /* width: 30%; */
    justify-content: center;
    margin-left: 1.5rem;
    margin-right: 1.5rem;
}
.illustration, .frame6-container{
    display: flex;
    align-items: center;
}
.frame6-container{
    padding: 1.3rem;
    /* width: 60% */
}
.frame6{
    width:80%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    text-align: left;
}
h2{
    color:#4D4D4D;
    font-size:2.4rem;
    margin: 0px;
}
p{
    color: #717171;
    font-size: .8rem;
}
</style>