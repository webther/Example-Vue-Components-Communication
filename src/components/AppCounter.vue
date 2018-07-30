<template>
  <div class="app-counter">
    <button v-on:click="increment">Increase</button> 
    &nbsp;&nbsp;
    <span>Counter: {{ counter }}</span>
  </div>
</template>

<script>
export default {
  name: 'AppCounter',
  data: function () {
    return {
      counter: 0
    }
  },
  methods: {
    increment:function () {
      this.counter += 1
      this.$emit('increment')
    }
  }
};
</script>

<style scoped>

</style>
