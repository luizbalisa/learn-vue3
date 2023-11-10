<script setup>
import Quiz from "@/components/Quiz/QuizMain.vue";
import { state } from "@/stores/quizStore";

</script>
<template>
  <main class="grid grid-cols-1 gap-32">
    <Quiz :quiz="state" />
  </main>
</template>
