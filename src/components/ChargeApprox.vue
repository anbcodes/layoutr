<template>
  <v-slider
    v-model="value"
    :min="0.5"
    :max="3.0"
    :step="0.1"
    thumb-label
    label="Charge approximation"
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
