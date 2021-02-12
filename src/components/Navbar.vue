<template>
  <div>
    <b-navbar type="dark" variant="info" class="bg-dark">
      <b-navbar-brand href="#">Merchant book</b-navbar-brand>
    </b-navbar>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Navbar extends Vue {
  @Prop() private msg!: string;
}
</script>
