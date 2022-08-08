<template>
  <ul class="my-6" v-if="windowWidth >= 1536">
    <li class="inline">
      <router-link class="text-lg mx-4 py-2.5 px-6 hover:bg-slate-500" to="/"
        >Home</router-link
      >
    </li>
    <li class="inline">
      <router-link
        class="text-lg mx-4 py-2.5 px-6 hover:bg-slate-500"
        to="/about"
        >About</router-link
      >
    </li>
    <li class="inline">
      <router-link
        class="text-lg mx-4 py-2.5 px-6 hover:bg-slate-500"
        to="/projects"
        >Projects</router-link
      >
    </li>
    <li class="inline">
      <router-link class="text-lg mx-4 py-2.5 px-6 bg-orange-600" to="/contact"
        >Contact</router-link
      >
    </li>
  </ul>
  <span v-else>Nav Menu</span>
</template>

<script>
import { ref } from "@vue/reactivity";
let windowWidth = ref("");
export default {
  setup() {
    window.addEventListener("resize", () => {
      windowWidth.value = window.innerWidth;
    });
    return { windowWidth };
  },
};
</script>

<style></style>
