<template>
  <div id="app">
    <Start/>
    <!-- <etap1/> -->
    <etap2/>
  </div>
</template>

<script>
import Start from "@/components/Start.vue"
// import etap1 from "@/components/etap_1.vue"
import etap2 from "@/components/Etap2"


export default {
  name: 'app',
  components: {
    Start,
    // etap1,
    etap2
  }
}
</script>

<style lang="scss">
body, html {
  margin: 0;
  padding: 0;
}

#app {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
  overflow-x: hidden;
}
</style>
