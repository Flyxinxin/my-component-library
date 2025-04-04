<template>
  <button :class="`btn ${color}`">{{ text }}</button>
</template>

<script setup>
defineProps({
  text: String,
  color: {
    type: String,
    default: 'primary',
  },
});
</script>

<style scoped>
.btn {
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 4px;
  font-size: 14px;
}

.primary {
  background-color: blue;
  color: white;
}

.secondary {
  background-color: gray;
  color: white;
}

.danger {
  background-color: red;
  color: white;
}
</style>