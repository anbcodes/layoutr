<template>
  <v-slider
    v-model="value"
    :min="0.00"
    :max="1.00"
    :step="0.01"
    thumb-label
    label="Radial force"
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
