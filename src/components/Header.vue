<script setup>
import { Icon } from "@iconify/vue";
import logo from "../assets/logo.png"
</script>

<template>
<header>
    <img :src="logo" alt="">
    <nav>
        <li><a href="">
            <Icon icon="material-symbols:search"/>
        </a></li>
        <li><a href="">Ínicio</a></li>
        <li><a href="">Galeria</a></li>
        <li><a href="">Favoritos</a></li>
        <li><a href="">
            <Icon icon="material-symbols:person"/>
        </a></li>
    </nav>
</header>
</template>

<style scoped lang="scss">
</style>