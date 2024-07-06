<script setup>
import { ref, computed } from "vue";
const input = ref('')

const score = ref(0)
const evaluation = computed(() => {
  return score.value > 3 ? 'good' : 'bad'
})
</script>
<template>
  <p>{{ input }}</p>
  <input v-model="input" type="text" name="" id="">

  <p>{{ evaluation }}</p>

  
</template>
<style>
</style>
