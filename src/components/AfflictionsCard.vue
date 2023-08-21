<script setup>
import { defineProps } from 'vue';
defineProps(["imageLink"])
/*const props = defineProps({
    image:{type:String,required:true}
})*/
</script>

<template>
    <div class="container">
        <img :src="imageLink" />
    </div>
    <!----<div class="container">
    <img :src="props.image" alt="logo" class="card-logo">*/
    </div>--->
</template>

<style scoped>
 .container{
    border-radius: 8px;
    background: #F5F5F5;
    display: flex;
    align-items: center;
    padding: 25px 24px;
    margin: 0 auto;
 }

 .container img{
   max-width: 98.97px;
   width: 100%;
max-height: 22.579px;
height: 100%;
flex-shrink: 0;

 }
</style>