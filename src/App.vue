<!-- src/App.vue -->
<template>
  <div id="app">
    <LabeledInput id="username" label-content="Username:" />
  </div>
</template>

<script>
import LabeledInput from './components/LabeledInput.vue';

export default {
  components: {
    LabeledInput
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
