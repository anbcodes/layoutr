<template>
  <v-combobox
    v-model="value"
    :items="['None', ...fields]"
    label="Size field"
    hide-details
    @change="change"
  ></v-combobox>
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
