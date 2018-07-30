<template>
  <div class="app-footer">
    Counter: {{ total }}
  </div>
</template>

<script>
export default {
  name: "AppFooter",
  props: ['total']
};
</script>

<style scoped>
.app-footer {
  background: lightblue;
  padding: 5px;
  margin-top: 15px;
}
</style>
