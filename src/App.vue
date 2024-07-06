<script setup>
import { ref } from "vue";
import ShowCount from '@/components/ShowCount.vue'
import ResetButton from '@/components/ResetButton.vue'
const count = ref(0)
function reset(value){
  count.value = value
}
</script>
<template>
<ShowCount :foo="count" />
<button @click="count++">add</button>
<ResetButton  @reset="reset"/>
</template>
<style>
</style>
