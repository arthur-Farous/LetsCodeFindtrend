<script setup>
import ButtonComponent from './ButtonComponent.vue';
import TheCardComponent from './TheCardComponent.vue';
import picture1 from '../assets/tBird.svg'
import picture4 from '../assets/last.svg'
import picture3 from '../assets/salute.svg'
import picture2 from '../assets/hello.svg'
</script>

<template>
   <div class="text-content">
    <h3>Minimize your tabs.</h3>
    <h3>Find the trends!</h3>
    </div>
    <div class="memory">
        <p>Don’t let your computer memories consumes all of those browser tabs.</p> 
        <p>Findtrend  let you gathers all of your favorite website into one place.</p>
    </div>
    <div class="start">
        <div class="btn-container">
        <ButtonComponent buttonText="Get Started 🔥" class="bt_1"/>
        </div>
        <div class="hero"><img src="../assets/img-hero.svg"/></div>
    </div>
    <div class="custom-cards">
      <div>
        <div class="crypto">
          <TheCardComponent  class="cd_1"  :cardImage ="picture1" cardText = "Cryptopunk - Search" />
        </div>
        <div class="Pop">
          <TheCardComponent  class="cd_2"  :card-image ="picture2" cardText = "Popular Design - Search" />
        </div>
      </div>
      <div>
        <div class="Pro">
          <TheCardComponent   class="cd_3"  :card-image = "picture3" cardText = "Product Design - Search" />
        </div>
        <div class="Elon">
          <TheCardComponent  class="cd_4"  :card-image = "picture4" cardText = "Elon Musk - Search" />
        </div>
      </div>
    </div>
</template>

<style scoped>
.text-content{
  display: flex;
  flex-direction: column;
  padding-top: 80px;
}
.text-content h3{
  color: #FFF;
text-align: center;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: 112%; /* 40.32px */
}

.memory{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-top: 16px;
  padding-bottom: 32px;
  padding-right: 44px;
  padding-left: 45px;
}

.memory p{
  color: #8B8B8B;
text-align: center;
font-family: Effra;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 150%; /* 21px */
}

.start{
   display: flex;
   justify-content: center;
   align-items: center;
   gap: 18px;
  }
  .hero{
    display: none;
  }
  .bt_1{
    background-color: #A8FF35;
    text-align: center;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: 140%;
  }

  .custom-cards{
    display: flex;
    flex-direction: column;
    padding: 60px 0px;
   }
   .cd_1{
    transform: rotate(-4deg);
   }
   .cd_2{
    transform: rotate(2deg);
   }

   .cd_3{
    transform: rotate(-2deg);
   }

   .cd_4{
    transform: rotate(4deg);
   }
  
@media (min-width: 1024px) {
  .text-content h3{
    font-size: 72px;
  }
  
  .memory {
    padding-top: 16px;
    padding-left: 387px;
    padding-right: 387px;
    padding-bottom: 40px;
  }

  .memory p{
    font-size: 18px;
  }
 
  .hero{
    display: block;
  }
  .bt_1{
    font-size: 18px;
  }

  .custom-cards{ 
    flex-direction: row;
    justify-content: center;
    padding: 100px 0px;}

.crypto{
    padding-right: 100px;
   }
   .Pop{
    padding-left: 100px;
   }
   .Pro{
    padding-right: 100px;
   }
   .Elon{
    padding-left: 150px;
   }

   .cd_1,.cd_2,.cd_3,.cd_4{
    font-size: 23.806px;
   }
  }
</style>
