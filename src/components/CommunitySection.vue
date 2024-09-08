<template>
    <div class="containery">
        <header>
            <h1 class="section-title">Manage your entire community in a single system</h1>
            <p class="description">Who is Nexcent suitable for?</p>
        </header>
        <div class="card-row">
            <CardBox class=box box="membership" />
            <CardBox class=box box="national" />
            <CardBox class=box box="clubs" />
        </div>
    </div>

</template>
<script setup lang="ts">
import CardBox from "@/components/CommunityCard.vue";
</script>
<style scoped>
.card-row{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    margin-bottom: 2.4rem;
}
.box{
    width: 25%;
}
@media (max-width: 767.98px)  {
    .card-row{
        flex-direction: column;
    }
    .box{
        width: 80%;
    }
}
</style>