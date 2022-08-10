<template>
  <section class="h-full w-full relative">
    <!-- Image -->
    <div
      class="absolute z-10 top-8 left-1/4 w-40 h-40 rounded-full shadow-md overflow-hidden lg:w-2/6 lg:h-full lg:rounded-none lg:shadow-none bg-orange-400* lg:top-0 lg:left-0"
    >
      <img
        src="./..//assets/img/me.jpg"
        alt="Profile Picture"
        class="object-cover h-full"
      />
    </div>
    <!-- Info -->
    <div
      class="absolute top-[118px] inset-x-0 right-1/4 w-80 h-80 px-7 shadow-md lg:shadow-none lg:w-4/6 lg:h-full lg:top-0 lg:right-0 lg:py-16 lg:px-0 flex flex-col justify-start items-center"
    >
      <h2
        class="text-2xl mt-20 mb-4 lg:mt-0 lg:text-5xl font-semibold text-[#191919]"
      >
        Hello there, I'm Vlad.
      </h2>
      <p class="text-base lg:text-3xl text-gray-400 mb-4 lg:mb-32 text-center">
        I'm a front-end developer, graphic designer and instructor
      </p>
      <ul class="text-center mb-32">
        <li>
          <router-link
            to="/about"
            class="block text-base lg:text-2xl bg-orange-400 py-3 lg:py-4 w-64 lg:w-96 mb-4 lg:mb-8 rounded-lg"
            >See who I am</router-link
          >
        </li>
        <li>
          <router-link
            to="/projects"
            class="block text-base lg:text-2xl bg-orange-400 py-3 lg:py-4 w-64 lg:w-96 rounded-lg"
            >See what I do</router-link
          >
        </li>
      </ul>
      <ul class="hidden lg:block">
        <li class="inline mr-8">
          <a
            href="https://www.facebook.com/goji.robe"
            target="_blank"
            rel="noopener noreferrer"
            ><i
              class="fa-brands fa-square-facebook fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline mr-8">
          <a
            href="https://www.instagram.com/vlad_crauciuc/"
            target="_blank"
            rel="noopener noreferrer"
            ><i
              class="fa-brands fa-square-instagram fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline mr-8">
          <a
            href="https://www.linkedin.com/in/vlad-crauciuc-344874205/"
            target="_blank"
            rel="noopener noreferrer"
            ><i
              class="fa-brands fa-linkedin fa-3x text-gray-400 hover:text-[#191919]"
            ></i
          ></a>
        </li>
        <li class="inline">
          <a
            href="https://github.com/VladCrauciuc"
            target="_blank"
            rel="noopener noreferrer"
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
