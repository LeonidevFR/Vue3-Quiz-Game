<template>
  <div class="bg-slate-900">
    <h1
      class="text-5xl font-bold text-center bg-gradient-to-r from-teal-500 to-teal-100 text-transparent bg-clip-text"
    >
      Welcome to my Quiz Game
    </h1>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const count = ref(0);

    // expose to template and other options API hooks
    return {
      count,
    };
  },

  mounted() {
    console.log(this.count); // 0
  },
};
</script>

<style scoped></style>
