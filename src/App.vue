<template>
  <nav
    class="bg-[#191919] flex items-center text-white min-h-[64px] sm:min-h-[80px]"
  >
    <div class="container mx-auto flex justify-between items-center">
      <Nav class="my-6" />
    </div>
  </nav>
  <main
    class="container mx-auto flex justify-center items center bg-blue-500 h-screen"
  >
    <router-view />
  </main>
  <footer></footer>
</template>

<script>
import Nav from "./components/Nav.vue";

export default {
  name: "App",
  components: { Nav },
  setup() {},
};
</script>

<style></style>
