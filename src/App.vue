<template>
  <div id="app">
    <Start/>
  </div>
</template>

<script>
import Start from "@/components/Start.vue"

export default {
  name: 'app',
  components: {
    Start
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
}

#app {
  display: flex;
  flex-direction: column;
}
</style>
