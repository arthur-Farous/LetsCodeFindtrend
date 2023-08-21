<script setup>
import ButtonComponent from './ButtonComponent.vue';

</script>


<template>

<nav>
      <div class="phone_nav">
        <img src="../assets/first-icon.svg" alt="" class="badge_1"/>
        <img src="../assets/hamburger.svg" alt="" class="menu_nav"/>
      </div>
      <div class="desktop_nav">
        <img src="../assets/trend-icon.svg" alt=""  class="badge_2"/>
      <ul>
        <li><a href="#">About</a></li>
        <li><a href="#">How it works</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Solution</a></li>
        <li><a href="#">Features</a></li>
      </ul>
      <div class="last-nav">   
        <a href="#">Login</a>
        <ButtonComponent buttonText="Register"/>
      </div>
      </div>
    </nav>
</template>


<style scoped>
nav{
    background-color: black;
    padding: 24px 18px;
}
.phone_nav{
    display: flex;
    justify-content: space-between;
}
.desktop_nav{
    display: none;
}

@media screen and (min-width: 1024px){

    .phone_nav{
        display: none;
    }
    .desktop_nav{
        display: flex;
        justify-content: space-between;
        align-items: center;
      padding: 28px 0px;
    }

    ul{ 
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
}

ul li{
    list-style: none;
    
}

a{
    text-decoration: none;
    color: #fff;
    gap: 10px;
    font-size: 18px;
}

.last-nav{ 
    display: flex;
    align-items: center;
    gap:40px ;
}
}
</style>