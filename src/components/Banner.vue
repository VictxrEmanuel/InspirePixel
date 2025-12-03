<script setup>
    import fotografo from "../assets/fotografo.png"
</script>

<template>
    <section class="banner">
        <div>
            <h1>Onde a paisagem vira
            <span>inspiração</span> .</h1>
            <p>Explore paisagens, cores e luzes que inspiram novas histórias através da fotografia.</p>
           
        </div>
        <img :src="fotografo" alt="" >
    </section>
</template>

<style scoped lang="scss">
.banner{
    // border: solid;
    display: flex;
    margin:2rem;
    justify-content: space-between

    h1{
        font-size: 4rem;
        

    }
    span{
            color: #E1306C;
            font-size: 4.5rem;
        }

    div{
        //border: solid;
        width:50%;
        align-items: center;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    
}
</style>