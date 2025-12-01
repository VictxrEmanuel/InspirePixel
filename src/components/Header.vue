<script setup>
import { Icon } from "@iconify/vue";
import logo from "../assets/logo.png"
</script>

<template>
<header>
    <img :src="logo" alt="">
    <nav>
        <ul>
            <li><a href="">
                <Icon icon="material-symbols:search"/>
            </a></li>

            <li><a href="">Ínicio</a></li>
            <li><a href="">Galeria</a></li>
            <li><a href="">Favoritos</a></li>

            <li><a href="">
                <Icon icon="material-symbols:person"/>
            </a></li>
        </ul>
    </nav>
</header>
</template>

<style scoped lang="scss">

header{
    
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin: 2rem;

    ul{
        gap: 1.5rem;
        display: flex;
        // border: solid;
        flex-wrap: wrap;
        list-style: none;
        align-items: center;

        a{
            text-decoration: none;
            color: black;
            
        }
    }
}
</style>