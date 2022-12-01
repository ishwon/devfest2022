<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="shadow-md bg-white sticky top-0 z-50">
    <nav class="max-w-6xl mx-auto py-4 px-4 md:px-0">
        <div class="flex justify-between items-center">
            <RouterLink to="/">
                <img src="/images/gdg-mauritius-logo.svg" class="h-3.5 md:h-5" />
            </RouterLink>

            <div class="hidden md:block">
              <ul class="flex flex-row gap-4 text-sm">
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">HOME</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">AGENDA</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">SPEAKERS</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><a href="https://gdg.community.dev/events/details/google-gdg-mauritius-presents-devfest-mauritius-2022/">REGISTER</a></li>
              </ul>
            </div>
        </div>
    </nav>
  </header>

  <RouterView />

  <footer class="bg-gray-100">
    <div class="max-w-6xl mx-auto">
      <nav class="py-6 lg:py-12 mx-4 lg:mx-0 flex flex-col md:flex-row gap-4 md:gap-0 justify-between border-b border-gray-300">
        <!-- About -->
        <div class="flex flex-col gap-1 text-gray-500">
          <h3 class="mb-2 text-xl text-gray-600 font-bold">About</h3>
          <a href="#" class="text-sm">GDG Mauritius</a>
          <a href="#" class="text-sm">Google Developers Group</a>
          <a href="#" class="text-sm">Meet the Team</a>
        </div>
        <!-- Past DevFests -->
        <div class="flex flex-col gap-1 text-gray-500">
          <h3 class="mb-2 text-xl text-gray-600 font-bold">Explore Past DevFests</h3>
          <a href="#" class="text-sm">DevFest Mauritius 2019</a>
          <a href="#" class="text-sm">DevFest Mauritius 2018</a>
        </div>
        <!-- Event Resources -->
        <div class="flex flex-col gap-1 text-gray-500">
          <h3 class="mb-2 text-xl text-gray-600 font-bold">Event Resources</h3>
          <a href="#" class="text-sm">Partnership Proposition</a>
          <a href="#" class="text-sm">Call for Papers</a>
        </div>
      </nav>

      <div class="py-4 mx-4 lg:mx-0 flex flex-row justify-between items-center">
        <img class="h-12" src="/images/logo-dark.png" />
        <a href="#" class="text-sm text-gray-500">Code of Conduct</a>
      </div>
    </div>
  </footer>
</template>
