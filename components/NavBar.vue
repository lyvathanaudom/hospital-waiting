<!-- components/Header.vue -->
<template>
  <header class="fixed bg-white left-0 right-0 py-4 px-[5%] ">
    <nav class=" mx-auto flex justify-between items-center">
      <div class="font-bold text-lg">YOUR WEBSITE</div>
      <div class="flex items-center gap-4 sm:gap-10">
        <!-- Desktop Navigation Links -->
        <div class="hidden sm:flex gap-10 items-center">
          <nuxt-link to="/" class="text-gray-500 hover:text-blue-500">Home</nuxt-link>
          <nuxt-link to="/about" class="text-gray-500 hover:text-blue-500">About Us</nuxt-link>
          <nuxt-link to="/work" class="text-gray-500 hover:text-blue-500">Work</nuxt-link>
          <nuxt-link to="/info" class="text-gray-500 hover:text-blue-500">Info</nuxt-link>
        </div>

        <!-- Get Started Button -->
        <Button text="Get Started" />

        <!-- Mobile Menu Button -->
        <button
          @click="toggleMenu"
          class="block sm:hidden text-gray-500 focus:outline-none"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16m-7 6h7"
            ></path>
          </svg>
        </button>
      </div>

      <!-- Mobile Navigation Links -->
      <div
        :class="{'hidden': !isMenuOpen, 'flex': isMenuOpen}"
        class="flex-col fixed sm:hidden gap-4 items-center bg-white shadow-md left-0 right-0 top-16 h-full py-10"
      >
        <nuxt-link to="/" class="text-lg text-gray-500 hover:text-blue-500">Home</nuxt-link>
        <nuxt-link to="/about" class="text-lg text-gray-500 hover:text-blue-500">About Us</nuxt-link>
        <nuxt-link to="/work" class="text-lg text-gray-500 hover:text-blue-500">Work</nuxt-link>
        <nuxt-link to="/info" class="text-lg text-gray-500 hover:text-blue-500">Info</nuxt-link>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
/* Add any additional styles here */
</style>