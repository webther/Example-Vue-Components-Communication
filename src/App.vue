<template>
  <div id="app">
    <app-header :total="total"></app-header>
    <app-counter :total="total" v-on:increment="incrementTotal"></app-counter>
    <app-footer :total="total"></app-footer>
</div>
</template>

<script>
import AppHeader from './components/AppHeader'
import AppFooter from './components/AppFooter'
import AppCounter from './components/AppCounter'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppCounter
  },
  data: function () {
    return {
      total: 10
    }
  },
  methods: {
    incrementTotal: function () {
      this.total += 1
    }
  }
};
</script>

<style>

</style>
