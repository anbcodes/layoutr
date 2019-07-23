<template>
  <v-checkbox v-model="value" label="Show Edges" hide-details @change="change"></v-checkbox>
</template>
<script>
export default {
  props: {
    value: Boolean
  },
  methods: {
    change() {
      this.$emit("input", this.value);
    }
  }
};
</script>
