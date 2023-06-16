<script setup>
import { ref } from "vue";
import ResumeWork from "../components/ResumeWork.vue"

const tecnologyimg = ref([
    [
        {
            name: "Html",
            urlimg: "/src/assets/html.png",
            urlWeb: "https://developer.mozilla.org/en-US/docs/Web/HTML",
        },
        {
            name: "Css",
            urlimg: "/src/assets/css.png",
            urlWeb: "https://developer.mozilla.org/en-US/docs/Web/CSS",
        },
        {
            name: "JavaScript",
            urlimg: "/src/assets/js.png",
            urlWeb: "https://developer.mozilla.org/en-US/docs/Web/JavaScript",
        },
        {
            name: "Vuejs",
            urlimg: "/src/assets/vue.png",
            urlWeb: "https://vuejs.org/",
        },
        {
            name: "Gsap",
            urlimg: "/src/assets/gsap.png",
            urlWeb: "https://e-johanherrera-f.netlify.app/img/gsap.png",
        },
        {
            name: "Asp.net MVC",
            urlimg: "/src/assets/asp.net.png",
            urlWeb: "https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/getting-started",
        },
    ],
    [
        {
            name: "PostgreSql",
            urlimg: "/src/assets/posgresql.png",
            urlWeb: "https://www.postgresql.org/",
        },
        {
            name: "SqlServer",
            urlimg: "/src/assets/sqlserver.png",
            urlWeb: "https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16",
        },
        {
            name: "jQuery",
            urlimg: "/src/assets/jQuery.png",
            urlWeb: "https://api.jquery.com/",
        },
        {
            name: "php",
            urlimg: "/src/assets/php.png",
            urlWeb: "https://www.php.net/docs.php",
        },
        {
            name: "mysql",
            urlimg: "/src/assets/mysql.php",
            urlWeb: "https://dev.mysql.com/doc/",
        },
    ],
    [
        {
            name: "GitHub",
            urlimg: "/src/assets/github.png",
            urlWeb: "https://docs.github.com/es",
        },
        {
            name: "Postman",
            urlimg: "/src/assets/postman.png",
            urlWeb: "https://www.postman.com/api-documentation-tool/",
        },
        {
            name: "C#",
            urlimg: "/src/assets/cshar.png",
            urlWeb: "https://learn.microsoft.com/en-us/dotnet/csharp/",
        },
    ],
]);

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
                <div class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight">
                    <h2 class="text-gray mb-10 font-semibold">
                        <i>Estas son, pero no se limitan a, la tecnología que uso para
                            construir aplicaciones del lado del cliente</i>
                    </h2>

                    <div class="w-16 inline-block mb-2 brand" v-for="img in tecnologyimg[0]">
                        <span :title="img.name"><a :href="img.urlWeb" target="_blank"><img :src="img.urlimg" :alt="img.name"
                                    class="h-12 inline brand__img" /></a></span>
                    </div>
                </div>

                <div class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight">
                    <h2 class="text-gray mb-10 font-semibold">
                        <i>Estas son, entre otras, la tecnología que uso para construir
                            rápido y aplicaciones de back-end</i>
                    </h2>

                    <div v-for="img in tecnologyimg[1]" class="w-16 inline-block brand">
                        <span :title="img.name"><a :href="img.urlWeb" target="_blank"><img :src="img.urlimg" :alt="img.name"
                                    class="h-12 inline brand__img" /></a></span>
                    </div>
                </div>
                <div class="mb-8 p-3 md:px-10 md:py-5 bg-kjColorLight dark:bg-kjColorBlack border-2 border-kjColorLight">
                    <h2 class="text-gray mb-10 font-semibold"><i>Otros</i></h2>
                    <div class="flex flex-wrap">

                        <div v-for="img in tecnologyimg[2]" class="w-16 brand md:mb-4">
                            <span :title="img.name"><a :href="img.urlWeb" target="_blank"><img :src="img.urlimg"
                                        :alt="img.name" class="h-12 brand__img" /></a></span>
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