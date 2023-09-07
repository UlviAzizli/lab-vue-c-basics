<script setup>
import { ref, computed } from "vue";
let num1 = ref(0);
let num2 = ref(0);

function sumNumber() {
  return Number(num1.value) + Number(num2.value);
}

const sum = computed(() => sumNumber());
</script>

<template>
  <input type="text" v-model="num1" id="number1" />
  <input type="text" v-model="num2" id="number2" />
  <label for="number1">insert numbert for sum: {{ sum }} </label>
  <p v-if="sum > 10">{{ sum }} sum is bigger than number 10</p>
</template>

<style></style>
