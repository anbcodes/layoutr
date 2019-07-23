<template>
  <v-slider
    v-model="value"
    :min="0.01"
    :max="1"
    :step="0.01"
    thumb-label
    label="Size"
    hide-details
    @change="change"
  />
</template>
<script>
export default {
  props: {
    value: Number
  },
  methods: {
    change() {
      this.$emit("input", this.value);
    }
  }
};
</script>
