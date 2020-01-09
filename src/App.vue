<template>
  <div id="app">
    <etap1/>
  </div>
</template>

<script>
import etap1 from "@/components/etap_1.vue"

export default {
  name: 'app',
  components: {
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
  width: 100vw;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>
