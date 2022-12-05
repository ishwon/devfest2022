<template>
  <main class="relative">
    <div class="max-w-6xl mx-auto pt-4 pb-16">
        <SpeakersComponent />
      </div>
  </main>
</template>

<script>
import SpeakersComponent from '../components/SpeakersComponent.vue';

export default {
	components: {
		SpeakersComponent,
	}
}
</script>
