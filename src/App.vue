<template>
  <div class="mx-auto flex flex-col justify-center w-screen h-screen">
    <nav
      class="bg-[#191919] flex items-center text-white min-h-[64px] sm:min-h-[80px] relative"
    >
      <div
        class="container mx-auto flex justify-between items-center relative*"
      >
        <Nav
          :showMobileNav="showMobileNav"
          :windowWidth="windowWidth"
          @openMobileNav="toggleMobileNav"
          @closeMobileNav="showMobileNav = false"
        />
        <MobileNav
          v-if="showMobileNav"
          @closeMobileNav="toggleMobileNav"
          v-click-outside="toggleMobileNav"
        />
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
import { onMounted, ref } from "@vue/runtime-core";
import Nav from "./components/Nav.vue";
import MobileNav from "./components/MobileNav.vue";
import vClickOutside from "click-outside-vue3";

let showMobileNav = ref(false);
let windowWidth = ref(window.innerWidth);

export default {
  name: "App",
  components: { Nav, MobileNav },
  directives: {
    clickOutside: vClickOutside.directive,
  },
  setup() {
    window.addEventListener("resize", () => {
      windowWidth.value = window.innerWidth;
    });

    function toggleMobileNav() {
      if (showMobileNav.value === true) {
        showMobileNav.value = false;
        console.log("mobile nav is hidden");
      } else if (showMobileNav.value === false) {
        showMobileNav.value = true;
        console.log("mobile nav is visible");
      }
    }

    return { showMobileNav, windowWidth, toggleMobileNav };
  },
};
</script>

<style></style>
