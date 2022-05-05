<template>
  <div class="p-2" :class="{ 'bg-gray-400': (row + column) % 2 == 1 }">
    <game-piece :player="boardState[row - 1][column - 1][0]" />
  </div>
</template>

<script lang="ts">
export default {
  props: {
    row: Number,
    column: Number,
  },

  setup() {
    const { value: boardState } = useBoardState();

    return {
      boardState,
    };
  },
};
</script>
