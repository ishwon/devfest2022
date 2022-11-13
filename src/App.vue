<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="shadow-md bg-white sticky top-0 z-50">
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div> -->
    <nav class="max-w-6xl mx-auto py-4">
        <div class="flex justify-between items-center">
            <RouterLink to="/">
                <img src="/images/gdg-mauritius-logo.svg" class="h-5" />
            </RouterLink>

            <ul class="flex flex-row gap-4 text-sm">
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">HOME</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/agenda">AGENDA</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">SPEAKERS</RouterLink></li>
                <li class="py-2 border-b-4 border-white hover:border-b-4 hover:border-green-600 hover:transition hover:ease-in-out duration-300"><RouterLink to="/">REGISTER</RouterLink></li>
            </ul>
        </div>
    </nav>
  </header>

  <RouterView />
</template>
