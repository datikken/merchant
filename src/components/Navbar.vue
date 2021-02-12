<template>
    <b-navbar type="dark" variant="info" class="bg-dark w-100 d-flex justify-content-between w-100">
      <b-container fluid="sm">
      <b-navbar-brand href="#">Merchant book</b-navbar-brand>
      <div id="nav">
        <router-link to="/" class="m-sm-4">Home</router-link>
        <router-link to="/about">About</router-link>
      </div>
      </b-container>
    </b-navbar>
</template>

<script lang="ts">
import {Component, Prop, Vue} from 'vue-property-decorator';

@Component
export default class Navbar extends Vue {
  @Prop() private msg!: string;
}
</script>

<style lang="scss">
.navbar {
  max-height: 250px;
}

#nav {
  a {
    color: #fff;
    text-decoration: none;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>