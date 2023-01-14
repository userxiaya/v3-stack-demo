<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="reload">刷新当前页面</button>
  </div>
</template>

<style>

</style>
<script lang="ts" setup>
import { onMounted } from 'vue';
const sleep = (time: number) => new Promise(resolve => setTimeout(resolve, time))
await sleep(1000)
defineProps<{
  reload: ()=>void
}>()
onMounted(() => {  
  console.log('about');

})
</script>
