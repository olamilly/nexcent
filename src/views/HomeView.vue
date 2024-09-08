<template>
  <div class="home">
    <HeaderComponent />
    <HeroSection />
    <ClientsSection />
    <CommunitySection />
    <UnlockSection />
    <AchievementSection />
    <CalendarSection />
    <CustomerSection />
    <MarketingSection />
    <FooterComponent />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HeaderComponent from '@/components/HeaderComponent.vue'; // @ is an alias to /src
import HeroSection from '@/components/HeroSection.vue';
import ClientsSection from '@/components/ClientsSection.vue';
import CommunitySection from '@/components/CommunitySection.vue';
import UnlockSection from '@/components/UnlockSection.vue';
import AchievementSection from '@/components/AchievementSection.vue';
import CalendarSection from '@/components/CalendarSection.vue';
import CustomerSection from '@/components/CustomerSection.vue';
import MarketingSection from '@/components/MarketingSection.vue';
import FooterComponent from '@/components/FooterComponent.vue';

export default defineComponent({
  name: 'HomeView',
  components: {
    HeaderComponent,
    HeroSection,
    ClientsSection,
    CommunitySection,
    UnlockSection,
    AchievementSection,
    CalendarSection,
    CustomerSection,
    MarketingSection,
    FooterComponent 
  },
});
</script>
