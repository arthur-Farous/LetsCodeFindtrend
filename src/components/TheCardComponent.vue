<script setup>
defineProps(['cardImage','cardText'])




</script>


<template>
    <div class="card-list">
        <img :src="cardImage"/>
        <p>{{ cardText }}</p>
        <img src="../assets/Terminate.png"/>
    </div>

</template>



<style>
.card-list{
  display: flex;
  background-color:#181818;
  padding: 14px 22px;
 justify-content: center;
 gap: 10px;
 max-width:299.413px;;
width: 100%;
margin: 0 auto;

}

.card-list p{
    color: #FFF;
text-align: center;
font-family: Roboto;
font-size: 23.806px;
font-style: normal;
font-weight: 400;
line-height: normal;
}

.card-list img{
    max-width: 27.259px;
    width: 100%;
  max-height: 27.259px;
height: 100%;

}
@media (min-width: 1024px) {
  .card-list p{
    font-size: 20.445px;
  }

  .card-list img{
    max-width: 31.742px;
    width: 100%;
   max-height: 31.742px;
   max-height: 100%;

    
  }
}
</style>