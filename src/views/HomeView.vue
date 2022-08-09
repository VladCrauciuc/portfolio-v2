<template>
  <section class="h-full w-full relative">
    <!-- Image -->
    <div class="w-2/6 h-full bg-green-500 absolute top-0 left-0"></div>
    <!-- Info -->
    <div
      class="w-4/6 h-full absolute top-0 right-0 py-16 flex flex-col justify-between items-center"
    >
      <h2 class="text-5xl font-semibold text-[#191919]">
        Hello there, I'm Vlad.
      </h2>
      <p class="text-3xl text-gray-400 mb-16">
        I'm a front-end developer, graphic designer and instructor
      </p>
      <ul class="text-center mb-16">
        <li>
          <router-link
            to="/about"
            class="block text-2xl bg-orange-400 py-4 w-96 mb-8 rounded-lg"
            >See who I am</router-link
          >
        </li>
        <li>
          <router-link
            to="/projects"
            class="block text-2xl bg-orange-400 py-4 w-96 rounded-lg"
            >See what I do</router-link
          >
        </li>
      </ul>
      <ul>
        <li class="inline mr-8">
          <a href="/"
            ><i
              class="fa-brands fa-square-facebook fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline mr-8">
          <a href="/"
            ><i
              class="fa-brands fa-square-instagram fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline mr-8">
          <a href="/"
            ><i
              class="fa-brands fa-linkedin fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline">
          <a href="/"
            ><i
              class="fa-brands fa-github fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: "HomeView",
  components: {},
};
</script>
