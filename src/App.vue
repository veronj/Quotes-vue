<template>
  <div class="container">
      <app-quote-grid :quotes="quotes"></app-quote-grid>
  </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';

export default {
  data () {
    return {
      quotes: [
        'The first quote',
        'A longer quote this time'
      ],
      maxQuotes: 10
    }
  },
  components: {
      appQuoteGrid: QuoteGrid
  }
}
</script>

<style>

</style>
