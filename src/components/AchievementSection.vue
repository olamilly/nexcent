<template>
    <div class="containery">
        <div class="text-box">
            <h3 id="large-text">
                <span style="color:#4D4D4D">Helping a local business</span>
                <!-- <br> -->
                <span style="color:#4CAF4F"> reinvent itself</span>
            </h3>
            <p id="small-text">
                We reached here with our hardwork and dedication.
            </p>
        </div>
        
        <div class="achievements">
            <div class="rowy">
                <div class="columny">
                    <div><MemberIcon /></div>
                    <div class="description">
                        <h4>2,468,719</h4>
                        <p>Members</p>
                    </div>
                </div>
                <div class="columny">
                    <div><ClubsIcon /></div>
                    <div class="description">
                        <h4>46,719</h4>
                        <p>Clubs</p>
                    </div>
                </div>
            </div>
            <div class="rowy">
                <div class="columny">
                    <div><EventsIcon /></div>
                    <div class="description">
                        <h4>846,719</h4>
                        <p>Event Bookings</p>
                    </div>
                </div>
                <div class="columny">
                    <div><PaymentIcon /></div>
                    <div class="description">
                        <h4>1,746,719</h4>
                        <p>Payments</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.containery{
    background-color: #F5F7FA;
    width: 100%;
    align-items: center;
    display: flex;
    padding-bottom: 3rem;
    padding-top: 3rem;
}
.text-box{
    width:50%;
    text-align: left;
    margin-left:4rem;
}
.achievements{
    width:70%;
}
@media(max-width: 767.98px){
    .containery{
        flex-direction: column;
    }
    .text-box{
        width: 100%;
    }
    .achievements{
        width: 100%;
        margin-top: 1rem; 
    }
}

#large-text{
    font-size:2.2rem;
    width:80%;
}
#small-text{
    font-size: .8rem;
}
.rowy{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.columny{
    display: flex;
    align-items: center;
}
.description{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
h4{
    margin-bottom: 2px;
    margin-top: 0px;
    font-size: 1rem;
}
p{
    margin:0px;
}
</style>
<script setup lang="ts">
import ClubsIcon from '@/assets/ClubsIcon.vue';
import EventsIcon from '@/assets/EventsIcon.vue';
import MemberIcon from '@/assets/memberIcon.vue';
import PaymentIcon from '@/assets/paymentIcon.vue';



</script>