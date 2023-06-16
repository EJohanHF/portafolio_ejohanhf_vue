<script setup>
import { ref } from "vue";

defineProps(['headerview' ])


const myProyect = ref([
    {
        id: 2,
        name: "Portafolio",
        urlimg: "/src/assets/portafoliojohan.png",
        urlWeb: "https://e-johanherrera-f.netlify.app/",
    },
]);
</script>
<template>
    <section :class="!headerview ?  'mt-12 md:mt-32 services' :''">
        <h1 v-if="!headerview" class="capitalize text-3xl md:text-4xl font-bold leading-none">
            Mis Trabajos
        </h1>
        <p v-if="!headerview" class="capitalize mt-2 text-lg">Algunos De mis Proyectos</p>
        <div v-if="!headerview"  class="mt-4 w-32 bg-kjColorPrime kj-border" data-v-24ddb798="">
            <div class="w-2 h-2 rounded-full bg-kjColorPrime kj-border__elips" data-v-24ddb798=""></div>
        </div>
        <div>
            <h1 class="mt-6 text-2xl font-bold capitalize">aplicaciones Web</h1>
            <div v-if="headerview"  class="mt-4 w-32 bg-kjColorPrime kj-border" data-v-24ddb798="">
            <div class="w-2 h-2 rounded-full bg-kjColorPrime kj-border__elips" data-v-24ddb798=""></div>
        </div>
            <div class="mt-8">
            <div>
                <!---->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 dark:text-kjColorGray">
                    <a v-for="dataPoyect in myProyect" href="https://e-johanherrera-f.netlify.app/" target="_blank">
                        <!-- Imagenenes Proyectos -->
                        <div class="relative pf-card rounded-lg">
                            <img :key="dataPoyect.id" :src="dataPoyect.urlimg" :alt="dataPoyect.name"
                                class="rounded-lg" />
                        </div>
                    </a>

                    <!-- </a> <a href="https://spasora.netlify.app/" target="_blank" >
                        <div class="relative pf-card rounded-lg" > <img
                            src="https://res.cloudinary.com/dwa1jtluu/image/upload/q_auto,f_auto/v1663252550/kenjimmy.me/333_kq5r5b.jpg"
                                alt="spasora" class="rounded-lg" ></div>
                          </a> <a href="https://bossbusworld.com/" target="_blank" >
                            <div class="relative pf-card rounded-lg" > <img
                                    src="https://res.cloudinary.com/dwa1jtluu/image/upload/q_auto,f_auto/v1663252537/kenjimmy.me/222_c7tsjz.jpg"
                                    alt="bossbus" class="rounded-lg" ></div>
                              </a>
                                  <div class="relative pf-card rounded-lg" > <img
                                      src="https://res.cloudinary.com/dwa1jtluu/image/upload/q_auto,f_auto/v1663252535/kenjimmy.me/112_xoqgia.jpg"
                                      alt="kenJimmy" class="rounded-lg" ></div> <a
                                    href="https://mazinomakeovers.netlify.app" target="_blank" >
                                    <div class="relative pf-card rounded-lg" > <img
                                        src="https://res.cloudinary.com/dwa1jtluu/image/upload/q_auto,f_auto/v1663252544/kenjimmy.me/444_a17rec.jpg"
                                        alt="mazino" class="rounded-lg" ></div>
                                  </a> <a href="https://flexicreate.com/" target="_blank" >
                                    <div class="relative pf-card rounded-lg" > <img
                                        src="https://res.cloudinary.com/dwa1jtluu/image/upload/q_auto,f_auto/v1663252564/kenjimmy.me/555_ahwodb.jpg"
                                                alt="flexicreate" class="rounded-lg" ></div>
                                              </a> -->
                    </div>
                    <a href="https://e-johanherrera-f.netlify.app/" target="_blank"> </a>
                </div>
                <a href="https://e-johanherrera-f.netlify.app/" target="_blank"> </a>
            </div>
            <a href="https://e-johanherrera-f.netlify.app/" target="_blank"> </a>
            <div class="max-w-xl shadow-2xl h-40 py-5 md:py-0 px-5 md:px-10 mt-10 md:flex justify-between items-center">
                <a href="https://e-johanherrera-f.netlify.app/" target="_blank">
                    <p class="text-lg font-bold mb-3 md:mb-0">
                        ¿Quieres saber más sobre mi profesión? 👉
                    </p>
                </a>
                <router-link to="/resume"  class="inline-block">
               
                    <svg id="btn"
                        xmlns="http://www.w3.org/2000/svg" width="220" height="60" viewBox="0 0 220 60" data-v-4227784c="">
                        <rect x="0" y="0" width="60" height="60" rx="30" ry="30" fill="#e45447" style="opacity: 0.4"
                            data-v-4227784c=""></rect>
                        <text transform="translate(50 38)" text-anchor="middle" font-size="20" fill="#000" font-weight="700"
                            style="fill: rgb(0, 0, 0)">
                            Mi CV
                        </text>
                    </svg>
            </router-link>
            </div>
        </div>
    </section>
</template>
