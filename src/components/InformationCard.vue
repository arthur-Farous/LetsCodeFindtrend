 <script setup>
import ButtonComponent from './ButtonComponent.vue';
defineProps(['h2','h5','h1','li1','li2','li3','li4','li5','li6'])
</script>


<template>
    
    <div class="session">
    <div class="inner-session">
        <div class="xoxo">
            <h1>{{ h2 }}</h1>
            <p>{{ h5 }}</p>
        </div>
        <hr>
        <div class="list">
            <h1>{{ h1 }}</h1>
            <ul>
                <li>{{ li1 }}</li>
                <li>{{ li2 }}</li>
                <li>{{ li3 }}</li>
                <li>{{ li4 }}</li>
                <li>{{ li5 }}</li>
                <li>{{ li6 }}</li>
            </ul>
            <ButtonComponent class="free"  buttonText="Start Free Trial"/>
        </div>
    </div>

</div>
        





</template>


<style scoped>
.session{
    background-color:black;
    display: flex;
    justify-content: center;
    margin: auto 0;
    align-items: center;
    border-radius: 16px;
    margin-top: 20px;
}
.free{
    display: flex;
    justify-content: center;
    background-color: black;
    color:white;
    border:none;
    font-size: 18px;
font-style: normal;
font-weight: 700;
line-height: 140%;
    margin-bottom:24px
}


.inner-session{
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: auto 0;
    align-items: center;
   
     
}
.xoxo h1{
    color: #000;
font-family: 'inter';
font-size: 32px;
font-style: normal;
font-weight: 400;
line-height: 100%; 
 padding-right:30px;
padding-left: 30px; 
}
 .xoxo{
    display:flex;
    flex-direction: column;
    gap: 24px;
    
}

hr {
    border: 2px solid #000; 
    margin-top: 24px;
    margin-bottom: 24px;
}
.xoxo h1{
    color: #000;
font-family: 'inter';
font-size: 36px;
font-style: normal;
font-weight: 400;
line-height: 100%;
padding-top: 30px;
padding-left: 30px;
padding-right:30px;
}
.list{
    display: flex;
    flex-direction: column;
    gap: 30px;
   
}

ul 
li{
    list-style: none
}
.list h1{
color: #000;
font-size: 60px;
font-style: normal;
font-weight: 400;
line-height: 100%; /* 60px */
}
ul{
    display: flex;
    flex-direction: column;
    gap:30px
}
li,.card p{
    color: #000;
font-family: 'inter';
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: 100%;
}

@media (min-width: 1024px) {
    .session{
        gap: 40px;
        margin-top:40px;
    }
}.xoxo h1{
    font-size:36px;
}

.xoxo p{
    font-size: 18px;
}

.list h1{
    font-size: 64px;
}

</style>