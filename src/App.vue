<template>
  <div class="container mx-auto flex flex-col justify-center items-center">
    <nav class="bg-slate-700 text-white w-screen flex justify-end">
      <Nav />
    </nav>
    <router-view />
  </div>
</template>

<script>
import Nav from "./components/Nav.vue";
import HomeView from "./views/HomeView.vue";
import AboutView from "./views/AboutView.vue";
import ProjectsView from "./views/ProjectsView.vue";
import ContactView from "./views/ContactView.vue";

export default {
  name: "App",
  components: { Nav, HomeView, AboutView },
  setup() {},
};
</script>

<style></style>
