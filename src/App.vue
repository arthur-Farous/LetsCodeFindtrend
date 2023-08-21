<script setup>
import TheNavbar from './components/TheNavbar.vue';
import ButtonComponent from './components/ButtonComponent.vue'
import TheSectionOne from './components/TheSectionOne.vue';
import TheCardComponent from './components/TheCardComponent.vue';
import TheSectionTwo from './components/TheSectionTwo.vue';
import TheSectionThree from './components/TheSectionThree.vue';
import AfflictionsCard from './components/AfflictionsCard.vue';
import TheSectionFour from './components/TheSectionFour.vue';
import TheSectionFive from './components/TheSectionFive.vue';
import TheSectionSix from './components/TheSectionSix.vue';
import TheFooter from './components/TheFooter.vue';
import InformationCard from './components/InformationCard.vue';
import TheArrowSection from './components/TheArrowSection.vue';
</script>

<template>
  <div>
  <section class="part_1">
    <TheNavbar/>
  <TheSectionOne/>
  </section>
  <TheSectionTwo/>
  <TheSectionThree/>
  <TheSectionFour/>
  <TheSectionFive/>
  <TheSectionSix/>
  <TheFooter/>

  
</div>
  
</template>

<style scoped>
.part_1{
  background-color: black;

}

@media (min-width: 1024px) {


}

</style>
