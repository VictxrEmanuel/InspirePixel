<script setup>
import { ref } from 'vue';
import Card from './Card.vue';
import axios from 'axios';

const imagens = ref([]);

    async function carregarImagens(){
        const res  = await axios.get('https://picsum.photos/v2/list?page3&limit=30');
        
        imagens.value = res.data;
        console.log(res);
    }

carregarImagens();
</script>
<template>
    <h2>Inspire-se</h2>
    <section class="inspire">
       <Card
        v-for="img in imagens"
        :imagem="img.download_url"
       />
    </section>
    
</template>
<style scoped lang="scss">
.inspire, h2{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 10px;
    margin: 2rem;
    // width: 100%;
    // height: 100%;
}
// .inspire {

//   display: grid;

//   grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

//   gap: 1.5rem;

//   margin: 0 2rem 2rem 2rem;

// }

</style>