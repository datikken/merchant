<template>
  <div id="app">
    <Navbar />
    <b-container fluid="sm" class="mt-4">
      <router-view/>
    </b-container>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Navbar from './components/Navbar.vue';

@Component({
  components: {
    Navbar,
  },
})

export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
