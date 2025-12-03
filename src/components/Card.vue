<script setup>
defineProps(["imagem"]);
</script>
<template>
    <div class="card">
        <img :src="imagem" alt="imagem">
    </div>
</template>
<style scoped lang="scss">
.card{
    //border: solid;
    width: 35vw;


    img{
        width: 100%;
        height: 100%;
        border-radius: 10px;
    }
}
</style>