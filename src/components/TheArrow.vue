<script setup>

defineProps(['imgLink','Url'])

</script>
<template>
    <div class="arrow_section">
        <img :src="imglink" alt="" class="v_1">
        <img :src="url" alt="" class="v_2">
    </div>
</template>

<style scoped>
     .arrow_section{
    display: flex;
    flex-direction: column;
    
}
.arrow_section .v_1{
    max-width: 28.394px;
    width: 100%;
   max-height: 34.446px;
   height: 100%;
flex-shrink: 0;
}


 .arrow_section .v_2{
    max-width: 61.195px;
    width: 100%;
transform: rotate(6deg);
}


@media (min-width: 1024px) {
   .arrow_section .v_1{
        max-width: 28.394px;
        height: 34.446px;
        transform: rotate(107.943deg);
        flex-shrink: 0;
    }

    .arrow_section .v_2{
        max-width: 71.888px;
        width: 100%;
transform: rotate(6deg);
    }
}

</style>