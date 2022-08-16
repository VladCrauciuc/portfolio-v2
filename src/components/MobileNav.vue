<template>
  <div
    class="absolute z-20 top-0 right-0 bg-[#191919] w-72 h-96 flex flex-col justify-center items-center px-4"
  >
    <span class="mr-4 cursor-pointer" @click="$emit('closeMobileNav')"
      ><i class="fas fa-xmark fa-2xl absolute top-8 right-4"></i
    ></span>
    <ul class="text-center block w-full">
      <li class="w-full">
        <router-link
          @click="$emit('closeMobileNav')"
          class="text-lg block w-full py-2 px-6 mb-3 hover:bg-gray-400"
          to="/"
          >Home</router-link
        >
      </li>
      <li class="w-full">
        <router-link
          @click="$emit('closeMobileNav')"
          class="text-lg block w-full py-2 px-6 mb-3 hover:bg-gray-400"
          to="/about"
          >About</router-link
        >
      </li>
      <li class="w-full">
        <router-link
          @click="$emit('closeMobileNav')"
          class="text-lg block w-full py-2 px-6 mb-3 hover:bg-gray-400"
          to="/projects"
          >Projects</router-link
        >
      </li>
      <li class="w-full">
        <router-link
          @click="$emit('closeMobileNav')"
          class="text-lg block w-full py-2 px-6 bg-orange-400"
          to="/contact"
          >Contact</router-link
        >
      </li>
    </ul>
  </div>
</template>

<script>
import { ref } from "@vue/reactivity";
import { watch } from "@vue/runtime-core";

export default {
  emits: ["closeMobileNav"],
  setup() {
    return {};
  },
};
</script>

<style></style>
