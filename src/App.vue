<template>
  <div id="app">
    <Start/>
    <etap1/>
  </div>
</template>

<script>
import Start from "@/components/Start.vue"
import etap1 from "@/components/etap_1.vue"

export default {
  name: 'app',
  components: {
    Start,
    etap1
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
  min-height: 100vh;
}
</style>
