<script setup>
import ButtonComponent from './ButtonComponent.vue';


</script>



<template>
    <section class="part_6">
        <div class="Join">
        <p>Join us on email for <span class="more">more trending topics</span></p>
        </div>
        <div class="butt">
        <ButtonComponent class="the" buttonText="Join Now"/>
        </div> 
    </section>
    
</template>



<style scoped>
.part_6{
    background-color: #a8ff35;
    
}
.Join{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-left: 18px;
    padding-right: 17px;
    gap: 40px;
    flex-direction: column;
   padding-top: 80px;
}
.more{
    color: #87D322;
}
.Join p{

color: #000;
text-align: center;

font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: 112%; /* 40.32px */

}

.butt{
    display: flex;
    padding:40px 135px 80px 134px;
}
.the{
    display: flex;
    flex-direction: column;
    /*justify-content: center;
    align-items: center;*/
    margin: 0 auto;
    background: #000;
    color: #FFF;
text-align: center;
font-size: 14px;
font-style: normal;
font-weight: 700;
line-height: 140%; /* 19.6px */
padding: 12px 24px;
}
    


@media (min-width: 1024px) {
    .Join p{
        font-size: 72px;
    }
.Join{
    padding-top: 140px;
    padding-bottom: 40px;
    padding-left: 350px;
    padding-right: 350px;
}
    .butt{
        justify-content: center;
        margin: 0 auto;
        padding-bottom: 140px;
        padding-right: 150px;
        padding-right: 150px;
    }

    .the{
        font-size: 18px;
     margin: 0 auto;
     padding: 16px 52.5px;
    }
}

</style>