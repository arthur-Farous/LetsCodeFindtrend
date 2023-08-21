<script setup>

</script>

<template>
  <div class="part_2">
    <h2>Open new tabs is sh*t</h2>
    <img class="mobile" src="../assets/littlebox.png"/>
    <img class="desktop" src="../assets/bigbox.png"/>
    <p>A solution for your browser tabs and don’t make your device get slower over time. Get ease and faster to discover a trend with just one tab.</p>
  </div>
</template>

<style>
.part_2{
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: #A8FF35;
  justify-content: center;
    align-items: center;
    gap: 34px;
    padding-top: 80px;
    /*padding-left: 10px;
    padding-right: 10px;*/
}

.part_2 h2{
  color: #000;
text-align: center;
font-size: 36px;
font-style: normal;
font-weight: 700;
line-height: 112%; /* 40.32px */
 
}

.part_2 p{
  color: #000;
text-align: center;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 150%; /* 21px */
padding: 0px 44px 80px 45px;
}

.desktop{
  display: none;
}

.part_2 img{
max-width: 250px;
width: 100%;
max-height: 118px;
height: 100%;
flex-shrink: 0;
}

@media (min-width: 1024px) {
  .mobile{
    display: none;
  }

  .desktop{
    display: block;
    justify-content: center;
  }

  .part_2{
    gap: 60px;
  }
.part_2 h2{
  font-size: 72px;
  padding-top: 140px;
}
.part_2 p{
  font-size: 18px;
  padding: 0px 387px 140px 387px;
}

.part_2 img{
  max-width: 502px;
  width: 100%;
  max-height: 202px;
  height: 100%;
  flex-shrink: 0;
}
}
</style>
