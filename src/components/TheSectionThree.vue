<script setup>
import AfflictionsCard from './AfflictionsCard.vue';
import image1 from '@/assets/Microsoft_icon.svg';
import image2 from '../assets/Allianz_icon.png';
import image3 from '../assets/UpWork_icon.png';
import image4 from '../assets/VOLVO_icon.png';
import image5 from '../assets/Grab.png';
import image6 from '../assets/verizon.png';
import image7 from '../assets/coin.png'
import image8 from '../assets/expe.png'
import image10 from '../assets/maga.png'
import image9 from '../assets/table.png'
import image11 from '../assets/CARRERA_icon.png';
import image12 from '../assets/Bonaza_icon.png';
import image13 from '../assets/WeTransfer_icon.png';
import image14 from '../assets/Suzuki_icon.png';
import image15 from '../assets/Algolia_icon.png';
import image16 from '../assets/Heineken_icon.png';




</script>


<template>
  <div class="part_3">
    <p>Findtrend helps you to increase your productivity and reduce your computer's 
        memory load,<span class="daily">an application that can fulfill your daily browsing needs.</span>
    </p>
    <h3>Findtrend make +1000 Startup grow</h3>
    <div class="brands">
      <AfflictionsCard class="qr" :imageLink="image1"/>
      <AfflictionsCard class="qr" :imageLink="image2"/>
      <AfflictionsCard class="qr" :imageLink="image3"/>
      <AfflictionsCard class="qr" :imageLink="image4"/>
      <AfflictionsCard class="qr" :imageLink="image5"/>
      <AfflictionsCard class="qr" :imageLink="image6"/>
      <AfflictionsCard class="qr" :imageLink="image7"/>
      <AfflictionsCard class="qr" :imageLink="image8"/>
      <AfflictionsCard class="qr" :imageLink="image9"/>
      <AfflictionsCard class="qr" :imageLink="image10"/>
      <AfflictionsCard class="qr" :imageLink="image11"/>
      <AfflictionsCard class="qr" :imageLink="image12"/>
      <AfflictionsCard class="qr" :imageLink="image13"/>
      <AfflictionsCard class="qr" :imageLink="image14"/>
      <AfflictionsCard class="qr" :imageLink="image15"/>
      <AfflictionsCard class="qr" :imageLink="image16"/>
    </div>
    </div>
    
  

 


</template>

<style scoped>
.part_3{
  display: flex;
  flex-direction: column;
  background-color: #fff;
  justify-content: center;
  align-items: center;
}


.part_3 p{
  color: #000;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
padding: 80px 22px 160px 22px;
}

.daily{
  color: #ADADAD;
}
.part_3 h3{
  color: #000;
text-align: center;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
padding-left: 20px;
padding-right: 20px;
padding-bottom: 32px;
}

.brands{
  display: grid;
    grid-template-rows: repeat(8, 1fr);
    grid-template-columns: 1fr 1fr;
    gap: 15px;
    margin: 0 auto;
    padding-bottom: 80px;
    margin: 0 auto;
}

.qr{
  /*display: flex;
  align-items: center;
    justify-content: center;*/
    max-width: 130px;
    width: 100%;
   
    padding: 25px 23px;
}
@media (min-width: 1024px) {
  .part_3 p{
    font-size: 64px;
    padding: 140px 140px 280px 140px;
    font-weight: 700;
  }

  .part_3 h3{
font-size: 64px;
font-weight: 700;
padding-bottom: 80px;
  }

  .brands{
    display: grid;
    grid-template-rows: repeat(4, 1fr);
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
    padding-bottom: 140px;
    justify-content: center;
  }
.qr{
  max-width: 266px;
  width: 100%;
  padding: 40px 55px;
}
}
</style>
