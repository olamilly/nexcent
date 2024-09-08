<template>
    <div class="containery">
        <div class="illustration">
            <UnlockLogo class="lo" />
        </div>
        <div class="frame6-container">
            <div class="frame6">
                <h2>The unseen of spending three years at Pixelgrade</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sit amet justo ipsum. Sed accumsan quam vitae est varius fringilla. Pellentesque placerat vestibulum lorem sed porta. Nullam mattis tristique iaculis. Nullam pulvinar sit amet risus pretium auctor. Etiam quis massa pulvinar, aliquam quam vitae, tempus sem. Donec elementum pulvinar odio.</p>
                <button class="medium">Learn More</button>
            </div>
        </div>
        
    </div>
</template>
<script setup lang="ts">
import UnlockLogo from '@/assets/UnlockLogo.vue';

</script>
<style scoped>
.containery{
    display: flex;
    margin-bottom: 2rem;
    align-items: center;
    
}
.illustration, .frame6-container{
    display: flex;
    align-items: center;
}
@media (max-width: 767.98px) {
    .containery{
        flex-direction: column;
    }
    .illustration, .frame6-container,.frame6{
        width:100%;
        justify-content: center;
    }
    .frame6{
        text-align: center;
    }
    .frame6-container{
        justify-content: center;
    }
}
.illustration{
    justify-content: center;
    /* width: 40% */
}


.frame6-container{
    padding: 1.3rem;
    /* width: 60% */
}
.frame6{
    width:85%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    text-align: left;
}
h2{
    color:#4D4D4D;
    font-size:2.4rem;
}
p{
    color: #717171;
    font-size: .8rem;
}
</style>