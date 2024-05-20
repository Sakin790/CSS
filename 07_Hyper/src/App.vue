<template>
  <div class="h-screen flex overflow-hidden">
    <div class="fixed w-64 bg-gray-800 dark:bg-gray-900 flex-col justify-between">
      <div class="h-16 bg-gray-700 dark:bg-gray-800 flex items-center justify-center">
      </div>
      <nav class="flex-grow overflow-auto px-4">
        <ul class="space-y-2">
          <li class="flex items-center p-2 rounded-md hover:bg-gray-700 dark:hover:bg-gray-800">
            <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M16 11.25h2m0-2.5h-2v-4a1 1 0 00-2-1h-2a1 1 0 00-2 1v4h-2m4-5v7a1 1 0 01-1 1h-2a1 1 0 01-1-1v-7a1 1 0 011-1h2z">
              </path>
            </svg>
            <span class="text-sm text-white dark:text-gray-200">nav 1</span>
          </li>
          <li class="flex items-center p-2 rounded-md hover:bg-gray-700 dark:hover:bg-gray-800">
            <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M9 17a2.25 2.25 0 100-4.5 2.25 2.25 0 000 4.5zM10 9.75v4.5m4-4.5v4.5m-4-4.5v4.5"></path>
            </svg>
            <span class="text-sm text-white dark:text-gray-200">nav 8</span>
          </li>
        </ul>
      </nav>
    </div>
    <div class="flex flex-col flex-1 overflow-y-auto px-4">
      <header class="h-16 bg-white border-b border-gray-200 dark:bg-gray-800 dark:border-gray-700">
      </header>
      <main class="flex-grow px-4 py-8">
        <div class="p-4 bg-white rounded shadow-md dark:bg-gray-800 dark:text-gray-200">
          Really long content here...
        </div>
      </main>
      <footer class="h-16 bg-gray-200 dark:bg-gray-800 flex items-center justify-center">
        <span class="text-sm text-gray-500 dark:text-gray-400">©2018 Created by Ant UED</span>
      </footer>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
const selectedKeys = ref(['4']);
</script>
