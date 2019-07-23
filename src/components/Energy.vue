<template>
  <v-slider
    v-model="value"
    :min="0.00"
    :max="1.00"
    :step="0.01"
    thumb-label
    :readonly="disabled"
    label="Energy"
    hide-details
  ></v-slider>
</template>
<script>
export default {
  props: {
    value: Number,
    disabled: Boolean
  },
  methods: {
    change() {
      this.$emit("input", this.value);
    }
  }
};
</script>
