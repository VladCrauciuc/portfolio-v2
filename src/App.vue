<template>
  <div class="container mx-auto flex flex-col justify-center items-center">
    <nav class="bg-slate-700 text-white w-screen flex justify-between">
      <div class="container mx-auto flex justify-end">
        <Nav />
      </div>
    </nav>
    <router-view />
  </div>
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
