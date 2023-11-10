<template>
  <div class="mt-8">
    <button @click="changeName" class="mb-4">{{ name }}</button >
    <ul class="flex gap-8 flex-col">
      <li><a href="">Get a Job</a></li>
      <li><a href="">Contact US </a></li>
    </ul>
  </div>
</template>

<script setup>
import { inject } from 'vue'
defineProps({
  quiz: Object
})

let {name, changeName} = inject('name');


</script>

<style lang="scss" scoped></style>
