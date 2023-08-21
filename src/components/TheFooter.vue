<script setup>

</script>


<template>
  <footer>
    <div class="foot">
        <img src="../assets/Frame.png"/>
    </div>
     <ul>
        <li><a href="#">Policy Privacy</a></li>
        <li><a href="#">Terms and Conditions</a></li>
        <li><a href="#">Contact Us</a></li>
        <li><a href="#">Careers</a></li>
    </ul>


  </footer>

</template>


<style scoped>
footer{
    display: flex;
    flex-direction: column;
    gap: 98px;
    padding-top: 62px;
}

.foot{
    padding-left: 62px;
}

ul{ 
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    gap: 40px;
    padding-left:100px;
    padding-right: 103px;
    
    
}

a{
    text-decoration: none;
    color: #000;
text-align: center;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: 100%; /* 18px */
align-items: center;
margin: 0 auto;
}
ul li{
    list-style: none;
    
    
}

@media (min-width: 1024px) {

 footer{
    flex-direction: row;
    justify-content:space-between;
    padding-top: 10px;
    padding-bottom: 10px;
    /*gap: 546px;*/
 }

 ul{
    flex-direction: row;
    justify-content: space-evenly;
 }
 .foot{
    padding-left: 80px;
    padding-top: 29px;
    padding-bottom: 30px;
 }
}

</style>