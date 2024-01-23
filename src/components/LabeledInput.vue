<!-- src/components/LabeledInput.vue -->
<template>
  <div>
    <label :for="id">{{ labelContent }}</label>
    <input v-model="inputValue" :id="id" type="text">
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  props: {
    id: {
      type: String,
      required: true
    },
    labelContent: {
      type: String,
      required: true
    }
  },
  setup(props) {
    const inputValue = ref('');

    return {
      inputValue
    };
  }
};
</script>
