<script setup>
import Test from "../components/Test.vue";
import { ref } from "vue";
const testProp = ref("Test Property");
</script>

<template>
  <main>
    <div>Testing Vue new page</div>
    <Test v-bind:testProp="testProp" />
    <div>Testing prop: {{ testProp }}</div>
  </main>
</template>

<style scoped>
main {
  background-color: lightblue;
}
</style>
