<template>
  <div class="page home-page">
    <h1>Home Page</h1>
    <md-button class="md-raised md-primary">Primary</md-button>
    <div v-for="h in headlines" :key="h.id">
      {{ headline }}
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ app }) {
    const topHeadlines = await app.axios.$get(
      `http://newsapi.org/v2/top-headlines?country=ukr`
    )
    return { headlines: topHeadlines.articles }
  }
}
</script>

<style lang="sass">

</style>