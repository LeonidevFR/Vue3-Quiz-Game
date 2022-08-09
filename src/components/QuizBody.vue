<template>
  <div class="bg-slate-900 h-full">
    <div v-for="(item, i) in questions" :key="i" class="text-white">
      {{ item.question }}
    </div>
  </div>
</template>

<script>
import { ref, onMounted } from "vue";
import Questions from "../assets/questions/quiz_questions.json";

export default {
  setup() {
    const questions = ref(["henlo"]);

    onMounted(() => {
      questions.value = Questions;
      console.log(questions.value[0]);
    });

    return {
      questions,
    };
  },
};
</script>

<style></style>
