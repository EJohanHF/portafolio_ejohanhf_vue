<template>
    <div>
      <div>
        
        <div>
          <!-- <PreLoader v-if="showHideSpinner"/> -->
  
          <div class="md:bg-kjColorLight dark:bg-kjColorBlack md:py-16">
            <div
              class="bg-white dark:bg-kjColorBlack md:max-w-6xl md:m-auto sm:rounded-lg p-2 md:p-8 text-kjColorGray md:shadow-2xl">
              <div class="md:flex">
                <AppHeader />
                <div class="md:flex-1">
                  <AppNav />
                  <div>
                    <RouterView />
                  </div>
                </div>
              </div>
            </div>
  
            <AppFooter/>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  
  import { RouterView } from "vue-router";
  import { ref, onMounted, onBeforeMount ,defineAsyncComponent} from 'vue';
  import AppNav from "../components/AppNav.vue";
  import AppHeader from "../components/AppHeader.vue";
  // import PreLoader from "./components/PreLoader.vue";
  import AppFooter from "../components/AppFooter.vue"
  
  
  
  
  
  
  
  // export default {
  //   components: {
  //     PreLoader,
  //     AppNav,
  //     AppHeader,
  //     AppFooter,
      
  // },
  //   beforeCreate() {
  //     this.showHideSpinner = true;
  //   },
  //   mounted() {
  //     this.showHideSpinner = false;
  //   },
  //   data() {
  //     return {
        
  //       showHideSpinner: true,
  //     };
  //   },
  // };
  </script>
  