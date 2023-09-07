<script setup>
import { ref } from "vue";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

const createCss = ref("click");

function clickTheme() {
  createCss.value = createCss.value === "click" ? "" : "click";
}
</script>

<template>
  <div :class="createCss">
    <Navbar></Navbar>
    <Footer></Footer>
    <button @click="clickTheme">Change color</button>
  </div>
</template>

<style>
.click {
  background-color: blueviolet;
  color: rgb(157, 158, 158);
}
</style>
