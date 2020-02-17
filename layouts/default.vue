<template>
  <div class="page-wrapper">
    <header>
      <nuxt-link class="md-primary" to="/">Home</nuxt-link>
      <nuxt-link class="md-primary" to="/about">About</nuxt-link>
    </header>
    <nuxt />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
header {
  padding: 20px 0;
  display: flex;
  justify-content: center;
}
</style>