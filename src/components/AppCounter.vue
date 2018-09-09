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
  props: {
    'total': {
      type: Number,
      required: true
    }
  },
  data: function () {
    return {
      counter: this.total
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
