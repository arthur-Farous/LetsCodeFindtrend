<script setup>
import InformationCard from './InformationCard.vue';
import ButtonComponent from './ButtonComponent.vue';
import TheArrowSection from './TheArrowSection.vue';

</script>



<template>
        <div class="deals"> 
        <div class="best">
          <p class="header">Get your best deal</p>
          <div class="underdeals">
              <span class="span">Monthly</span>
              <img src="../assets/toggleButton.png" alt=""  class="toggle"/>
              <p class="year">yearly</p>
              <img src="../assets/Group 42.png" class="disk"/>
          </div> 
          </div>
          <div class="show"><img src="../assets/suit10.png" alt="" class="arrow"/></div>
          
          <div class="card-container">
          
          <InformationCard   class="numero_1" h2="Personal" h5="Special First packet for all"  h1="$8/month" li1="&#x2713;Up to 5 page each group" li2="&#x2713;Up to 10 group page" li3="&#x2713;5days group page saved" />
          <InformationCard class="numero_2" h2="Regular" h5="Recommended for for Personal Pro" h1="$20/month" li1="&#x2713;Up to 15 page each group" li2="&#x2713;download page up to 20page" li3="&#x2713;Up to 10 group page" li4="&#x2713;15days group page saved"/> 
          <InformationCard class="numero_3" h2="Personal" h5="Special First packet for all"    h1="$48/month" li1="&#x2713;Unlimited group pages" li2="&#x2713;Unlimited download page" li3="&#x2713;Unlimited page each group" li4="&#x2713;Customize sorting group pages" li5="&#x2713;customize group page name"  li6="&#x2713;30 days group page saved"/>
        
        </div>
        
      </div>

</template>




<style scoped>
.deals{
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-items: center;
    background-color: black;
    padding-top: 80px;
         padding-left: 20px;
         padding-right: 20px;
         margin: 0 auto;


}

.best{
  display: flex;
  flex-direction: column;
    padding-left: 18px;
    padding-right: 18px;
  gap: 32px;
}
.underdeals{
    display: flex;
    margin: o auto;
    justify-content: center;
    gap: 24px;
    padding-left: 41px;
    padding-right:41px;
    
   
}

.disk{
  display: none;
}
.toggle{
  max-width: 104px;
  width: 100%;
max-height: 44px;
height:100%;
flex-shrink: 0;
}
.header{
  color: #FFF;
text-align: center;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
    
}

.span{
  color: #FFF;
font-family: Inter;
font-size: 18px;
font-style: normal;
font-weight: 500;
line-height: normal;
}

.show{
  display:flex;
  flex-direction: column;
  align-items: center;
justify-content: center;
padding-left: 180px;
}
.arrow{
  
  max-width: 63.368px;
  width: 100%;
 max-height: 66.265px;
  height: 100%;
flex-shrink: 0;



}

.year{
  color: #F5F5F5;
font-size: 18px;
font-style: normal;
font-weight: 500;
line-height: normal;
}

.card-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  gap: 24px;
  margin-bottom: 80px;
  

}
.numero_1{
   margin:0 auto
}
.numero_1,.numero_3{
  background-color: #FAFAFA;
  color: #000;
  padding-left :30px ;
  padding-right:30px;
  max-width: 360px;
        width: 100%;
       max-height: 640px;
       height: 100%;
       flex-shrink: 0;
       margin:0 auto
}
.numero_2{
  background-color: #a8ff35;
  padding: 30px 30px;
  max-width: 360px;
        width: 100%;
       max-height: 640px;
       height: 100%;
       flex-shrink: 0;
       margin:0 auto
}

@media (min-width: 1024px) {
  .disk{display: block;}
  .card-container{
    /*padding-left: 10px;*/
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
  }
  .show{ display: none;}
   
  .best{
    gap: 40px;
  }
  .span{
font-size: 24px;
font-weight: 500;

  }


  .header{
font-size: 64px;
font-weight: 700;

  }
  .year{
font-size: 24px;
opacity: 0.5;
  }
}

@media (min-width: 1024px) and (max-width: 1170px) {
  .numero_1,.numero_2,.numero_3{
    max-width: 320px;
    width: 100%;
    max-height: 600px;
    height: 100%;
flex-shrink: 0;
padding: 20px;
  }
}

</style>