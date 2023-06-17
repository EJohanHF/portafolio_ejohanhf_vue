<script setup>
import { RouterView } from "vue-router";
import AppNav from "./components/AppNav.vue";
import AppHeader from "./components/AppHeader.vue";


    
    
</script>

<template>
  <div>
    <div>
      <div>
        <div class="md:bg-kjColorLight dark:bg-kjColorBlack md:py-16">
          <div
            class="bg-white dark:bg-kjColorBlack md:max-w-6xl md:m-auto sm:rounded-lg p-2 md:p-8 text-kjColorGray md:shadow-2xl"
          >
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
        </div>
      </div>
    </div>
  </div>
</template>
