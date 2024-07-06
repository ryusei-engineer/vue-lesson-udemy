<script setup>
// import { ref } from "vue";
defineEmits(['reset'])
</script>
<template>
<button @click="$emit('reset', 100)">reset</button>
</template>
<style>
</style>
