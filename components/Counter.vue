<template>
  <div>
    {{ counter }}
    <button @click="counter++">+</button>
    <button @click="counter--">-</button>
  </div>
</template>

<script setup>
const counter = useState("count", () => 0);
</script>
