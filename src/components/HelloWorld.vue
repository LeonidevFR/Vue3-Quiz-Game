<template>
  <div class="justify-center flex bg-yellow-300 items-center h-screen">
    <div class="text-4xl">Hello 👋🏼</div>
    <div>{{ props.msg }}</div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  msg: String,
});
</script>

<style scoped></style>
