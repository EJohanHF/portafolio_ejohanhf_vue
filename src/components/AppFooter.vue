<script setup></script>
<template>
  <div class="md:max-w-6xl md:m-auto p-2 md:p-8 text-kjColorGray">
    <footer class="mt-10 md:flex">
      <div
        class="uppercase text-xs md:w-1/4 text-center mb-3 md:mb-0 md:text-left"
      >
        <router-link
          to="/"
          aria-current="page"
          class="nuxt-link-exact-active nuxt-link-active"
          ><img
            src="@/assets/logo.webp"
            alt="logo"
            class="w-12 pb-2 inline-block"
        /></router-link>
      </div>
      <div class="text-center md:w-2/4 mb-3 md:mb-0">
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
      <div class="uppercase text-center text-xs md:w-1/4">
        <p class="py-1 px-2">© 2023 J. all rights reserved</p>
      </div>
    </footer>
    <div class="h-3 mt-5 flex">
      <div class="h-full w-1/3 bg-kjColorPrime"></div>
      <div class="h-full w-1/3 bg-kjColorGold"></div>
      <div class="h-full w-1/3 bg-kjColorPrimeLight"></div>
    </div>
  </div>
</template>
