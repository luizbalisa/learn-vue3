<template>
   <div class="border mt-8 p-2 text-lg text-gray-900 ">
        <QuizHeader />

        <QuizQuestion />

        <QuizFooter :quiz="quiz" />
    </div>
</template>

<script setup>
import QuizHeader from './QuizHeader.vue';
import QuizQuestion from './QuizQuestion.vue';
import QuizFooter from './QuizFooter.vue';
import { provide, ref } from 'vue';

defineProps({quiz: Object});

let name = ref('Ola Mundo');

provide('name',{
    name,
    changeName: () => name.value = "Change Name"
});
</script>

<style lang="scss" scoped></style>