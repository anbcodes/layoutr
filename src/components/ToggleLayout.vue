<template>
  <v-btn block @click="click">{{ layoutRunning ? 'Stop' : 'Start' }} layout</v-btn>
</template>
<script>
export default {
  props: {
    layoutRunning: Boolean
  },
  methods: {
    click(v) {
      this.$emit("click", v);
    }
  }
};
</script>
