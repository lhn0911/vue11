<template>
  <div>
    <p>age: {{ age }}</p>
    <button @click="handleIncreaseAge">Increase age</button>
    <B4Children :age="age"></B4Children>
  </div>
</template>

<script setup>
import B4Children from "./B4con.vue";
import { ref } from "vue";

const age = ref(1);
const handleIncreaseAge = () => {
  age.value++;
};
</script>

<style></style>
