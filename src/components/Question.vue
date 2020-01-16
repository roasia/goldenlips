<template>
  <div class="question">

    <h2 class="question__title">{{ title }}</h2>
    <p class="question__text"> {{ text }}</p>
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
.question {
  text-align: center;
  margin-bottom: 3em;
  &:last-child {
    margin-bottom: 0;
  }

  &__title{
    margin-top: 0;
    color:gold;
    text-transform: uppercase;

  }

  &__text{
    margin-bottom: 0;
    color:white;
    text-transform: uppercase;
  }
}
</style>