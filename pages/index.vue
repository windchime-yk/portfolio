<template>
  <div class="container">
    <w-header />
    <main id="main" class="main">
      <about-contents />
      <skill-contents />
      <works-contents />
    </main>
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'

export default defineComponent({})
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 100vh;
  margin: 0 auto;
}
.main {
  width: 100%;
  max-width: 1000px;
  padding-top: 100px + $header-height;
  margin-top: -$header-height;
  @include mq('tb') {
    width: 90%;
    padding-top: 50px;
    margin-top: 0;
    margin-right: auto;
    margin-left: auto;
  }
}
</style>
