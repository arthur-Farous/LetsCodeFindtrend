 <script setup>
import ButtonComponent from './ButtonComponent.vue';
defineProps(['h2','h5','h1','li1','li2','li3','li4','li5','li6'])
</script>


<template>
    
    <div class="session">
    <div class="inner-session">
        <div class="xoxo">
        <h1>{{ h2 }}</h1>
        <p>{{h5}}</p>
        </div>
        <hr>
        <div class="list">
            <h1>{{ h1 }}</h1>
            <ul>
                <li>.{{li1}}</li>
                    <li>{{li2}}</li>
                    <li>{{ li3 }}</li>
                    <li>{{li4}}</li>
                    <li>{{ li5 }}</li>
                    <li>{{ li6 }}</li>
                    
                
            </ul>
            <ButtonComponent class="free" buttonText="Start Free trial"/>
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

}
.free{
    display: flex;
    justify-content: center;
    background-color: black;
    color:white;
    border:none
}
.inner-session{
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: auto 0;
    align-items: center;
    gap:56px;
    padding:30px 30px 30px 30px;
}
.xoxo h1{
    color: #000;
font-family: 'inter';
font-size: 32px;
font-style: normal;
font-weight: 400;
line-height: 100%; 
}
 .xoxo{
    display:flex;
    flex-direction: column;
    gap:14px
}
.xoxo h1{
    color: #000;
font-family: 'inter';
font-size: 36px;
font-style: normal;
font-weight: 400;
line-height: 100%;
}
.list{
    display: flex;
    flex-direction: column;
    gap:27px
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
    
}


</style>