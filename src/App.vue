<template>
  <div class="mx-auto flex flex-col justify-center w-screen h-screen">
    <nav
      class="bg-[#191919] flex items-center text-white min-h-[64px] sm:min-h-[80px]"
    >
      <div class="container mx-auto flex justify-between items-center">
        <Nav />
      </div>
    </nav>
    <main
      class="container mx-auto flex justify-center items-start h-full py-16*"
    >
      <router-view />
    </main>
    <footer class="bg-red-500* flex flex-col items-center">
      <span class="py-3">Copyright &copy; Vlad Crauciuc, 2022</span>
      <router-link
        to="/contact"
        class="bg-orange-400 py-4 w-full text-center text-white"
        >Want to work together? Contact me</router-link
      >
    </footer>
  </div>
</template>

<script>
import { onMounted } from "@vue/runtime-core";
import Nav from "./components/Nav.vue";

export default {
  name: "App",
  components: { Nav },
  setup() {
    function resetHeight() {
      document.body.style.height = window.innerHeight + "px";
    }
    window.addEventListener("resize", resetHeight);
    resetHeight();
  },
};
</script>

<style></style>
