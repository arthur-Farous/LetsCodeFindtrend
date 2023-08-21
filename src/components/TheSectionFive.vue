<script setup>
import InformationCard from './InformationCard.vue';
import ButtonComponent from './ButtonComponent.vue';
import TheArrowSection from './TheArrowSection.vue';
import file1 from '../assets/Arrow 5.svg';
import file2 from '../assets/Save.svg';
</script>



<template>
 <div class="Best">
          <h1>Get your Best Deal</h1>
          <div class="date"><p>Monthly</p>
          <img src="../assets/toggleButton.png" alt=""/>
          <p>Yearly</p>
          <div class="double"><TheArrowSection     :imgLink="file1"  :Url="file2 " /></div>
          </div>
          <div class="card-container">
          
          <InformationCard   class="numero_1" h2="Personal" h5="Special First packet for all"  h1="$8/month" li1="&#x2713;Up to 5 page each group" li2="&#x2713;Up to 10 group page" li3="&#x2713;5days group page saved"/>
          <InformationCard class="numero_2" h2="Regular" h5="Recommended for for Personal Pro" h1="$20/month" li1="&#x2713;Up to 15 page each group" li2="&#x2713;download page up to 20page" li3="&#x2713;Up to 10 group page" li4="&#x2713;15days group page saved"/> 
          <InformationCard class="numero_3" h2="Personal" h5="Special First packet for all"    h1="$48/month" li1="&#x2713;Unlimited group pages" li2="&#x2713;Unlimited download page" li3="&#x2713;Unlimited page each group" li4="&#x2713;Customize sorting group pages" li5="&#x2713;customize group page name"  li6="&#x2713;30 days group page saved"/>
        
        </div>
        
      </div>

</template>




<style scoped>

.Best{
    display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap:20px;
  background-color:black;
  padding-top: 80px;
  padding-bottom: 80px;
}
.card-container{
    display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 auto;
  gap:40px;
  padding-top: 80px;
  }

  .numero_1,.numero_3{
    background-color:white;
  border-radius: 20px;
 /* max-width: 360px;
width:100%;
max-height:602px;
height: 100%;*/
  padding:30px 30px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: auto 0;
    align-items: center;
    gap:56px
  }

 .numero_2{
    background-color: #A8FF35;
  border-radius: 20px;
  /*max-width: 360px;
width:100%;
max-height:602px;
height: 100%;*/
padding:20px 20px 20px 20px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: auto 0;
    align-items: center;
    gap:56px
 }

 .double img{
  display:flex;
  align-items: center;
  max-width: 104px;
  width:100%;
  max-height: 52px;
  height: 100%;
}
.Best h1{
  color:white;
  display: flex;
  justify-content: center;
}

@media (min-width: 1024px) {
.Best{
    justify-content: center;
    align-items: center;
    
}

.Best h1{
padding-top: 140px;
}
.card-container{
    flex-direction: row;
    display: flex;
  flex-direction: row;
  gap:20px;
  justify-content: center;
  padding-top: 20px;
  padding-left:50px;
  padding-right: 50px;
}

.numero_1{
max-width: 360px;
width: 100%;
height: 100%;
max-height: 640px;
flex-shrink: 0;
}

}
</style>