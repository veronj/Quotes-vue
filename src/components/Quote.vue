<template>
    <div class="col-sm-6 col-lg-3">
            <div class="panel panel-default">
                <div class="panel-body quote">
                    <slot></slot>
                </div>
            </div>
    </div>
</template>

<script>
import Quote from './Quote.vue';
    export default {
        props: ['quotes'],
        components: {
            appQuote: Quote
        }
    }
</script>

<style>
    .panel-body {
        font-family: 'Arizonia', cursive;
        font-size: 24px;
        color: black;
    }

    .quote {
        cursor: pointer;
    }

    .quote:hover {
        background-color: burlywood;
    }
</style>
