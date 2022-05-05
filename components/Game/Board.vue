<template>
  <div class="inline-flex flex-col bg-gray-200 shadow-sm">
    <game-row v-for="index in 8" :key="index" :row="index" />
  </div>
</template>
