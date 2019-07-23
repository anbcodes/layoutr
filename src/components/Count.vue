<template>
  <div>{{ nodeCount }} nodes, {{ edgeCount }} edges</div>
</template>
<script>
export default {
  props: {
    nodeCount: Number,
    edgeCount: Number
  }
};
</script>
