<template>
  <router-link class="text-3xl ml-4 2xl:ml-0 sm:text-4xl" to="/"
    ><span>vlad</span><span class="font-bold">crauciuc</span></router-link
  >
  <ul v-if="windowWidth > 1024">
    <li class="inline">
      <router-link class="text-lg mx-3 py-2 px-6 hover:bg-gray-400" to="/"
        >Home</router-link
      >
    </li>
    <li class="inline">
      <router-link class="text-lg mx-3 py-2 px-6 hover:bg-gray-400" to="/about"
        >About</router-link
      >
    </li>
    <li class="inline">
      <router-link
        class="text-lg mx-3 py-2 px-6 hover:bg-gray-400"
        to="/projects"
        >Projects</router-link
      >
    </li>
    <li class="inline">
      <router-link
        class="text-lg mr-4 2xl:mr-0 ml-3 py-2 px-6 bg-orange-400"
        to="/contact"
        >Contact</router-link
      >
    </li>
  </ul>
  <span v-else class="mr-4 cursor-pointer"
    ><i class="fas fa-bars fa-xl"></i
  ></span>
</template>

<script>
import { ref } from "@vue/reactivity";
let windowWidth = ref(window.innerWidth);
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
