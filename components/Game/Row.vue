<template>
  <div class="flex">
    <game-item v-for="index in 8" :key="index" :row="row" :column="index" />
  </div>
</template>

<script lang="ts">
export default {
  props: {
    row: Number,
  },
};
</script>
