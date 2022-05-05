<template>
  <div
    class="w-6 h-6 rounded-full"
    :class="{ 'bg-black': player == 1, 'bg-white': player == 2 }"
  ></div>
</template>

<script>
export default {
  props: {
    player: Number,
  },
};
</script>
