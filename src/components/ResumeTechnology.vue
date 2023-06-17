<script setup>
import { ref, watchEffect } from "vue";
import ResumeWork from "../components/ResumeWork.vue";

const tecnologyimg = ref([]);

watchEffect(async ()=> {
  
  const newTecnologyimg = [
  [
    {
      name: "Html",
      urlimg: (await(import('/src/assets/html.webp'))).default,
      urlWeb: "https://developer.mozilla.org/en-US/docs/Web/HTML",
    },
    {
      name: "Css",
      urlimg: (await(import('/src/assets/css.webp'))).default,
      urlWeb: "https://developer.mozilla.org/en-US/docs/Web/CSS",
    },
    {
      name: "JavaScript",
      urlimg: (await(import('/src/assets/js.webp'))).default,
      urlWeb: "https://developer.mozilla.org/en-US/docs/Web/JavaScript",
    },
    {
      name: "Vuejs",
      urlimg: (await(import('/src/assets/vue.webp'))).default,
      urlWeb: "https://vuejs.org/",
    },
    {
      name: "Gsap",
      urlimg: (await(import('/src/assets/gsap.webp'))).default,
      urlWeb: "https://e-johanherrera-f.netlify.app/img/gsap.webp",
    },
    {
      name: "Asp.net MVC",
      urlimg: (await(import('/src/assets/asp.net.webp'))).default,
      urlWeb:
        "https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/getting-started",
    },
  ],
  [
    {
      name: "PostgreSql",
      urlimg: (await(import('/src/assets/posgresql.webp'))).default,
      urlWeb: "https://www.postgresql.org/",
    },
    {
      name: "SqlServer",
      urlimg: (await(import('/src/assets/sqlserver.webp'))).default,
      urlWeb:
        "https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16",
    },
    {
      name: "jQuery",
      urlimg: (await(import('/src/assets/jQuery.webp'))).default,
      urlWeb: "https://api.jquery.com/",
    },
    {
      name: "php",
      urlimg: (await(import('/src/assets/php.webp'))).default,
      urlWeb: "https://www.php.net/docs.php",
    },
    {
      name: "mysql",
      urlimg: (await(import('/src/assets/mysql.webp'))).default,
      urlWeb: "https://dev.mysql.com/doc/",
    },
  ],
  [
    {
      name: "GitHub",
      urlimg: (await(import('/src/assets/github.webp'))).default,
      urlWeb: "https://docs.github.com/es",
    },
    {
      name: "Postman",
      urlimg: (await(import('/src/assets/postman.webp'))).default,
      urlWeb: "https://www.postman.com/api-documentation-tool/",
    },
    {
      name: "C#",
      urlimg: (await(import('/src/assets/cshar.webp'))).default,
      urlWeb: "https://learn.microsoft.com/en-us/dotnet/csharp/",
    },
  ],
  ]
  tecnologyimg.value = newTecnologyimg
})
</script>
<template>
  <div>
    <h1 class="mt-6 text-2xl font-bold capitalize">Tecnologias que uso</h1>
    <div class="mt-4 w-32 bg-kjColorPrime kj-border">
      <div class="w-2 h-2 rounded-full bg-kjColorPrime kj-border__elips"></div>
    </div>
    <!-- Tenologias usadas from  -->
    <div class="mt-8">
      <div>
        <div
          class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight"
        >
          <h2 class="text-gray mb-10 font-semibold">
            <i
              >Estas son, pero no se limitan a, la tecnología que uso para
              construir aplicaciones del lado del cliente</i
            >
          </h2>

          <div
            class="w-16 inline-block mb-2 brand"
            v-for="img in tecnologyimg[0]"
          >
            <span :title="img.name"
              ><a :href="img.urlWeb" target="_blank"
                ><img
                  :src="img.urlimg"
                  :alt="img.name"
                  class="h-12 inline brand__img" /></a
            ></span>
          </div>
        </div>

        <div
          class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight"
        >
          <h2 class="text-gray mb-10 font-semibold">
            <i
              >Estas son, entre otras, la tecnología que uso para construir
              rápido y aplicaciones de back-end</i
            >
          </h2>

          <div v-for="img in tecnologyimg[1]" class="w-16 inline-block brand">
            <span :title="img.name"
              ><a :href="img.urlWeb" target="_blank"
                ><img
                  :src="img.urlimg"
                  :alt="img.name"
                  class="h-12 inline brand__img" /></a
            ></span>
          </div>
        </div>
        <div
          class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight"
        >
          <h2 class="text-gray mb-10 font-semibold"><i>Otros</i></h2>
          <div class="flex flex-wrap">
            <div v-for="img in tecnologyimg[2]" class="w-16 brand md:mb-4">
              <span :title="img.name"
                ><a :href="img.urlWeb" target="_blank"
                  ><img
                    :src="img.urlimg"
                    :alt="img.name"
                    class="h-12 brand__img" /></a
              ></span>
            </div>
          </div>
        </div>
      </div>

      <ResumeWork />
    </div>
    <!-- <h1 class="mt-6 text-2xl font-bold capitalize">experience</h1>
                <div class="mt-4 w-32 bg-kjColorPrime kj-border">
                  <div class="w-2 h-2 rounded-full bg-kjColorPrime kj-border__elips"></div>
            </div> -->
  </div>
</template>

<style>
.brand__img:hover {
  transform: scale(1.3);
  -webkit-filter: none;
  filter: none;
}
</style>
