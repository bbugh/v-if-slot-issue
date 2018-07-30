<template>
  <div id="app">
    <conditional-slot :showSlot="false">
      {{ example.should.not.be.called }}
    </conditional-slot>
  </div>
</template>

<script>
import ConditionalSlot from './components/ConditionalSlot.vue'

export default {
  name: 'app',
  components: {
    ConditionalSlot
  },
  data: () => ({
    example: {}
  })
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
