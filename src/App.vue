<script setup>
import { ref, defineAsyncComponent } from 'vue';
import loadingComponent from './components/PreLoader.vue';
// import PageLayout from './page/page.vue'

const PageLayout = defineAsyncComponent({
  loader: () => {
    return new Promise((resolve,reject)=>{
      setTimeout(()=>{
        resolve(import('./page/page.vue'));
      },2000);
    })
  },
  loadingComponent:loadingComponent,

})


const show = ref(false)
</script>
<template>
  <PageLayout/>
</template>