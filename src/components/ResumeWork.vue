<script setup>
import cv from '@/assets/CV-JOHAN.pdf'

</script>

<template>
  <h1 class="mt-6 text-2xl font-bold capitalize">experience</h1>
  <div class="mt-4 w-32 bg-kjColorPrime kj-border">
    <div class="w-2 h-2 rounded-full bg-kjColorPrime kj-border__elips"></div>
  </div>

  <div class="ml-8 mt-10">
    <h3 class="font-bold">
      <a href="https://sos-tic.com/" target="_blank"><u>Sos Tic</u></a>
    </h3>
    <p class="mt-2">Programador Junior (Full-time)</p>
  </div>

  <div class="ml-8 mt-8">
    <h3 class="font-bold">
      <a href="http://www.union-bit.com/" target="_blank"><u>Union Bit</u></a>
    </h3>
    <p class="mt-2">Analista Programador (Full-time)</p>
  </div>

  <div class="ml-8 mt-8">
    <h3 class="font-bold">
      <a href="https://fiberpro.com.pe/" target="_blank"><u>Fiber Pro</u></a>
    </h3>
    <p class="mt-2">Auxiliar Del Noc (Full-time)</p>
  </div>

  <div class="flex justify-between items-center flex-wrap">
    <a
      :href="cv"
      download="CV-JohanHerreraFaudno.pdf"
      target="_blank"
      >
      <button
        class="p-2 mt-10 mb-10 md:mb-0 w-50 text-center text-white font-semibold bg-kjColorSecondary shadow-lg cursor-pointer my-cv"
      >
        <p style="vertical-align: inherit">
          <p style="vertical-align: inherit"> Descargar mi currículum </p>
          </p>
      </button></a
    >
  </div>
</template>
