<template>
    <div class="row">
        <div class="col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
            <label>Quote</label>
            <textarea class="form-control" rows="3" v-model="quote"></textarea>
        </div>
        <div class="col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
            <button class="btn btn-primary" @click.prevent="addQuote">Add quote</button>
        </div>
    </div>
</template>

<script>

    export default {
      data: function() {
          return {
              quote: ''
          }
      },
      methods: {
          addQuote() {
              this.$emit('quoteAdded', this.quote);
              this.quote = '';
          }
      }
    }
</script>

<style>

</style>
