<template>
  <v-slider
    v-model="value"
    :min="0"
    :max="50"
    :step="1"
    thumb-label
    label="Charge strength"
    hide-details
    @change="change"
  ></v-slider>
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
