<script setup>
import { ref } from "vue";

const props = defineProps(["testProp"]);

const name = ref("Andy");

function nameChange() {
  name.value = "AndyButton";
}
</script>

<style scoped>
div {
  background-color: yellow;
}
</style>

<template>
  <button @click="nameChange">Click to Change Name</button>
  <div>Testing prop in child: {{ props.testProp }}</div>
  <div>{{ name }}</div>
</template>
