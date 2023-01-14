<script setup lang="ts">
import { onMounted } from 'vue';
import { useRouter } from 'vue-router'
const router = useRouter()
onMounted(() => {
  console.log('home')
})
const next = () => {
  router.push('/about')
}
</script>

<template>
  <div @click="next" style="width: 100%; height: 100%;">home</div>
</template>
