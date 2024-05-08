<template>
  <nav class="bg-gray-800 flex justify-between items-center px-4 py-2 lg:px-8">
    <a href="#" class="text-white text-xl font-bold">Event Management</a>
    <ul class="hidden lg:flex space-x-4">
      <li><a href="#" class="text-white hover:text-gray-400">Home</a></li>
      <li><a href="#" class="text-white hover:text-gray-400">About</a></li>
      <li><a href="#" class="text-white hover:text-gray-400">Services</a></li>
      <li><a href="#" class="text-white hover:text-gray-400">Contact</a></li>
    </ul>
    <button @click="toggleMenu" class="lg:hidden text-white focus:outline-none">
      <svg
        v-if="!isOpen"
        class="h-6 w-6"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          d="M4 6h16v12H4zm2-2a2 2 0 1 0-4 0 2 2 0 0 0 4 0zM16 14a2 2 0 1 0-4 0 2 2 0 0 0 4 0z"
        ></path>
      </svg>
      <svg
        v-else
        class="h-6 w-6"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path d="M6 18L18 6M6 6l12 12"></path>
      </svg>
    </button>
  </nav>
</template>

<script>
  export default {
    data() {
      return {
        isOpen: false,
      };
    },
    methods: {
      toggleMenu() {
        this.isOpen = !this.isOpen;
      },
    },
  };
</script>

<style scoped></style>
