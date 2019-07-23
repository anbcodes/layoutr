<template>
  <v-combobox v-model="value" :items="fields" label="Y field" hide-details @change="change" />
</template>
<script>
export default {
  props: {
    value: String,
    fields: Array
  },
  methods: {
    change() {
      this.$emit("input", this.value);
    }
  }
};
</script>
