<script setup>
import { ref } from "vue";
const title = "vue-lesson"
let int = ref(0)
function increment() {
  int.value++
}
</script>
<template>
<h1>{{ title }}</h1>
<p>{{ int }}</p>
<button @click="increment">add</button>
</template>

<style>
</style>
