<template>
  <main class="relative">
    <div class="max-w-6xl mx-auto pt-4 pb-16">
      <SessionsComponent />
    </div>
  </main>
</template>

<script>
import SessionsComponent from "../components/SessionsComponent.vue";

export default {
  components: {
    SessionsComponent,
  },
};
</script>
