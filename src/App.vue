<script setup>
import { ref, reactive } from "vue";
const message = ref('<h1>hello</h1>')

const URL = ref('https://ja.vuejs.org/')
const int = ref(0)
function increment(){
  int.value++
}
</script>
<template>
  <p>{{ message }}</p>
  <p v-html="message"></p>

  <a v-bind:href="URL">Vue.js</a>
  <p>{{ int }}</p>
  <button v-on:click="increment">click</button>
</template>
<style>
</style>
