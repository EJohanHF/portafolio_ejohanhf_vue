<script setup>
import { ref } from "vue";
import AppNavSidebar from "./AppNavSidebar.vue"
const toggleDarkMode = ref(document.documentElement.className === "dark-mode");

const ChangeDarMode = () => {
  toggleDarkMode.value = document.documentElement.classList.toggle("dark-mode");
  toggleDarkMode.value
    ? (localStorage.theme = "light")
    : (localStorage.theme = "dark-mode");
};


</script>
<template>
  <nav>
    <div class="hidden md:flex">
      <div class="text-kjColorGray text-sm md:flex-1">
        <!-- Correo Nav -->
        <div class="font-bold md:ml-4 inline-block py-1 px-2 hover:f-link">
          <a href="mailto:E.Johan.Herrera.F@Gmail.com"
            ><svg
              aria-hidden="true"
              focusable="false"
              data-prefix="fas"
              data-icon="envelope"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 512 512"
              class="text-lg mr-1 svg-inline--fa fa-envelope fa-w-16"
            >
              <path
                fill="currentColor"
                d="M502.3 190.8c3.9-3.1 9.7-.2 9.7 4.7V400c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V195.6c0-5 5.7-7.8 9.7-4.7 22.4 17.4 52.1 39.5 154.1 113.6 21.1 15.4 56.7 47.8 92.2 47.6 35.7.3 72-32.8 92.3-47.6 102-74.1 131.6-96.3 154-113.7zM256 320c23.2.4 56.6-29.2 73.4-41.4 132.7-96.3 142.8-104.7 173.4-128.7 5.8-4.5 9.2-11.5 9.2-18.9v-19c0-26.5-21.5-48-48-48H48C21.5 64 0 85.5 0 112v19c0 7.4 3.4 14.3 9.2 18.9 30.6 23.9 40.7 32.4 173.4 128.7 16.8 12.2 50.2 41.8 73.4 41.4z"
                class=""
              ></path>
            </svg>
            E.Johan.Herrera.F@Gmail.com
          </a>
        </div>
        <!-- Dark Page Desktop -->
        <span
          @click="ChangeDarMode"
          class="cursor-pointer ml-10 dark:text-kjColorGray"
        >
          <svg
            aria-hidden="true"
            focusable="false"
            data-prefix="fas"
            data-icon="sun"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
            class="text-lg ml-1 svg-inline--fa fa-sun fa-w-16"
          >
            <path
              fill="currentColor"
              d="M256 160c-52.9 0-96 43.1-96 96s43.1 96 96 96 96-43.1 96-96-43.1-96-96-96zm246.4 80.5l-94.7-47.3 33.5-100.4c4.5-13.6-8.4-26.5-21.9-21.9l-100.4 33.5-47.4-94.8c-6.4-12.8-24.6-12.8-31 0l-47.3 94.7L92.7 70.8c-13.6-4.5-26.5 8.4-21.9 21.9l33.5 100.4-94.7 47.4c-12.8 6.4-12.8 24.6 0 31l94.7 47.3-33.5 100.5c-4.5 13.6 8.4 26.5 21.9 21.9l100.4-33.5 47.3 94.7c6.4 12.8 24.6 12.8 31 0l47.3-94.7 100.4 33.5c13.6 4.5 26.5-8.4 21.9-21.9l-33.5-100.4 94.7-47.3c13-6.5 13-24.7.2-31.1zm-155.9 106c-49.9 49.9-131.1 49.9-181 0-49.9-49.9-49.9-131.1 0-181 49.9-49.9 131.1-49.9 181 0 49.9 49.9 49.9 131.1 0 181z"
              class=""
            ></path>
          </svg>
        </span>
      </div>

      <!-- Rutas -->
      <div>
        <router-link to="/"
          ><button class="focus:outline-none py-1 px-2 capitalize hover:f-link">
            <svg
              aria-hidden="true"
              focusable="false"
              data-prefix="fas"
              data-icon="file"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 384 512"
              class="text-lg mr-1 svg-inline--fa fa-file fa-w-12"
            >
              <path
                fill="currentColor"
                d="M224 136V0H24C10.7 0 0 10.7 0 24v464c0 13.3 10.7 24 24 24h336c13.3 0 24-10.7 24-24V160H248c-13.2 0-24-10.8-24-24zm160-14.1v6.1H256V0h6.1c6.4 0 12.5 2.5 17 7l97.9 98c4.5 4.5 7 10.6 7 16.9z"
                class=""
              ></path>
            </svg>
            Inicio
          </button></router-link
        >

        <router-link to="/proyect"
          ><button class="focus:outline-none py-1 px-2 capitalize hover:f-link">
            <svg
              aria-hidden="true"
              focusable="false"
              data-prefix="fas"
              data-icon="file"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 384 512"
              class="text-lg mr-1 svg-inline--fa fa-file fa-w-12"
            >
              <path
                fill="currentColor"
                d="M224 136V0H24C10.7 0 0 10.7 0 24v464c0 13.3 10.7 24 24 24h336c13.3 0 24-10.7 24-24V160H248c-13.2 0-24-10.8-24-24zm160-14.1v6.1H256V0h6.1c6.4 0 12.5 2.5 17 7l97.9 98c4.5 4.5 7 10.6 7 16.9z"
                class=""
              ></path>
            </svg>
            Proyectos
          </button></router-link
        >
        <router-link to="/resume"
          ><button class="focus:outline-none py-1 px-2 capitalize hover:f-link">
            <svg
              aria-hidden="true"
              focusable="false"
              data-prefix="fas"
              data-icon="file"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 384 512"
              class="text-lg mr-1 svg-inline--fa fa-file fa-w-12"
            >
              <path
                fill="currentColor"
                d="M224 136V0H24C10.7 0 0 10.7 0 24v464c0 13.3 10.7 24 24 24h336c13.3 0 24-10.7 24-24V160H248c-13.2 0-24-10.8-24-24zm160-14.1v6.1H256V0h6.1c6.4 0 12.5 2.5 17 7l97.9 98c4.5 4.5 7 10.6 7 16.9z"
                class=""
              ></path>
            </svg>
            Curriculum
          </button></router-link
        >
      </div>
    </div>

    <!-- Dark Color movil -->
    <span @click="ChangeDarMode" class="absolute left-0 top-0 ml-24 mt-3 md:hidden"
      ><span class="cursor-pointer ml-10 dark:text-kjColorGray"
        ><svg
          aria-hidden="true"
          focusable="false"
          data-prefix="fas"
          data-icon="sun"
          role="img"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 512 512"
          class="text-lg ml-1 svg-inline--fa fa-sun fa-w-16"
        >
          <path
            fill="currentColor"
            d="M256 160c-52.9 0-96 43.1-96 96s43.1 96 96 96 96-43.1 96-96-43.1-96-96-96zm246.4 80.5l-94.7-47.3 33.5-100.4c4.5-13.6-8.4-26.5-21.9-21.9l-100.4 33.5-47.4-94.8c-6.4-12.8-24.6-12.8-31 0l-47.3 94.7L92.7 70.8c-13.6-4.5-26.5 8.4-21.9 21.9l33.5 100.4-94.7 47.4c-12.8 6.4-12.8 24.6 0 31l94.7 47.3-33.5 100.5c-4.5 13.6 8.4 26.5 21.9 21.9l100.4-33.5 47.3 94.7c6.4 12.8 24.6 12.8 31 0l47.3-94.7 100.4 33.5c13.6 4.5 26.5-8.4 21.9-21.9l-33.5-100.4 94.7-47.3c13-6.5 13-24.7.2-31.1zm-155.9 106c-49.9 49.9-131.1 49.9-181 0-49.9-49.9-49.9-131.1 0-181 49.9-49.9 131.1-49.9 181 0 49.9 49.9 49.9 131.1 0 181z"
            class=""
          ></path></svg></span
    ></span>
    
    <AppNavSidebar/>
    
 
  </nav>
</template>
