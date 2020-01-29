<template>
  <div class="question"> 
    <p class="question_title">{{ title }}</p>
    <p class="question_text"> {{ text }}</p>
  </div>
</template>

<script>
export default {
  name: "Question",
  props: {
    title: String,
    text: String
  }
}
</script>

<style lang="scss" scoped>
  p {
    margin: 0;
    padding: 0;
  }
  .question_title {
    text-transform: uppercase;
    color: rgb(235, 181, 33);
    font-size: 2rem;
    padding-top: 9vh;
    font-weight: 900;
  }
  .question_text {
     font-size: 1.3rem;
     padding-top: 1.5vh;
     line-height: 1.6rem;
  }
</style>