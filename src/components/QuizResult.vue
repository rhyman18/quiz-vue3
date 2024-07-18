<script setup>
const { quizQuestionLength, numberOfCorrectAnswers } = defineProps([
  'quizQuestionLength',
  'numberOfCorrectAnswers'
])
</script>

<template>
  <section class="results">
    <p>Score</p>
    <h1>{{ numberOfCorrectAnswers }}/{{ quizQuestionLength }}</h1>
    <RouterLink to="/">Go Back</RouterLink>
  </section>
</template>

<style scoped>
.results {
  text-align: center;
  padding: 100px 0;
}

p {
  font-size: 25px;
}

h1 {
  font-size: 80px;
}
</style>
