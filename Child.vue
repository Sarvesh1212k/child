<script setup>
defineProps(['name'])

const emit = defineEmits(['message'])
</script>

<template>
  <h2>Child Component</h2>

  <p>Name: {{ name }}</p>

  <button @click="emit('message', 'Hello Parent')">
    Send Message
  </button>
</template>