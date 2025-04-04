<template>
  <button>{{ text }}</button>
</template>

<script setup>
defineProps({
  text: String,
});
</script>