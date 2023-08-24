<script setup>
import ButtonComponent from './ButtonComponent.vue';




</script>


<template>
<section class="part_4">
  <h2>All platform connect to Findtrend</h2>
  <div class="media-handles">
        <img class="view" src="../assets/fBook.svg"/>
        <img class="view  bird" src="../assets/tBird.svg"/>
        <img class="view" src="../assets/Pia.svg"/>
        <img class="view" src="../assets/Mia.svg"/>
  </div>
  <div class="desktop-handles">
        <img class="dk" src="../assets/fb_logo.svg"/>
        <img class="dk   bird" src="../assets/t_logo.svg"/>
        <img class="dk" src="../assets/pipa.svg"/>
        <img class="dk" src="../assets/Mima.svg"/>
        <img class="dk" src="../assets/doll.svg"/>
        <img class="dk" src="../assets/wk.svg"/>
        <img class="dk" src="../assets/linked-in.svg"/>
  </div>
  <div class="twitter-phone">
        <img src="../assets/Mobile_tweet1.png"/>
        <img src="../assets/Mobile_tweet2.png"/>
        <img src="../assets/Mobile_tweet3.svg"/>
    </div>
    <div class="twitter-desktop">
        <img src="../assets/Mobile_tweet1.png"/>
        <img src="../assets/Mobile_tweet2.png"/>
        <img src="../assets/Mobile_tweet3.svg"/>
    </div>
    <ButtonComponent class="Btn" buttonText="View More Trend"/>
</section>

</template>


<style scoped>

.part_4{
    padding-bottom: 80px;
    
}
.part_4 h2{
    color: #000;
text-align: center;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
padding-bottom: 32px;
}

.media-handles{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 16px;
    padding-bottom: 32px;
}
.desktop-handles{
  display: none;
}
.view{
    border-radius: 8px;
    background: #FFF;
    padding: 16.5px;
    width: 64px;
}

.bird{
    background: #A8FF35;
}

.twitter-phone{
    display: flex;
    flex-direction: column;
    gap: 16px;
    padding: 0px 18px 32px 18px
}

.twitter-desktop{
    display: none;
}


.Btn{
    display: flex;
    /*justify-content: center;
    align-items: center;*/
    background: #000;
    margin: 0 auto;
    color: #FFF;
    text-align: center;
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: 140%;
    padding: 16px 24px;
    
    
}
@media (min-width: 1024px) {
    .part_4 h2{
font-size: 64px;
font-weight: 700;

    }
 .part_4{
    padding-bottom: 140px;
 }
    .media-handles{
        display: none;
    }

    .desktop-handles{
        display: block;
        border-radius: 8px;
        background: #FFF;
        padding: 20px;
        display: flex;
    align-items: center;
    justify-content: center;
    gap: 24px;
    padding-bottom: 77px;
    }

    .dk{
     padding: 32px;
    }
    .bird{
        background-color: #A8FF35;
    }
    .twitter-phone{
        display: none;
    }

    .twitter-desktop{
        display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 40px;
    padding: 0px 320px 80px 320px;
    }

    .Btn{
        font-size: 14px;
        padding: 16px 32px;
    }

}

</style>