<script setup>
import HomeHeader from '../components/HomeHeader.vue';
import HomeMyInfo from '../components/HomeMyInfo.vue';
import MyProyect from '../components/MyProyect.vue'

const headerview = false

</script>

<template>

    <HomeHeader />
    <HomeMyInfo/>
    <MyProyect
    :headerview = "headerview"/>

</template>
