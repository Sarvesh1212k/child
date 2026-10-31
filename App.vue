<script setup>
import Child from './Child.vue'

function showMessage(msg) {
  alert(msg)
}
</script>

<template>
  <h1>Parent Component</h1>

  <Child name="Sarvesh" @message="showMessage" />
</template>