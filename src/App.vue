<template>
  <div id="app">
    <Etap2/>
  </div>
</template>

<script>
import Etap2 from "@/components/Etap2"
export default {
  name: 'app',
  components: {
    Etap2
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
  flex-direction: column;
}
</style>
