<script setup>
import Card from './Card.vue';
</script>
<template>
    <h2>Inspire-se</h2>
    <section class="inspire">
        <Card imagem="https://i.pinimg.com/736x/cc/0d/37/cc0d3781240d0fbfe57194dd56898c88.jpg"/>
        <Card imagem="https://img.freepik.com/fotos-gratis/ponte-de-madeira-para-a-praia-durante-o-por-do-sol_181624-18247.jpg?semt=ais_hybrid&w=740&q=80" />
    </section>
    
</template>
<style scoped lang="scss">
.inspire, h2{
    display: flex;
    justify-content: space-between;
    gap: 10px;
    margin: 2rem;
}

</style>