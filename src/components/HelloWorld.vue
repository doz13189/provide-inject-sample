<template>
  {{ userLocation }}
  {{ userGeolocation }}
</template>

<script lang="ts">
import { defineComponent, inject } from 'vue';

export default defineComponent({
  setup() {
    const userLocation = inject('location', 'The Universe')
    const userGeolocation = inject('geolocation')

    return {
      userLocation,
      userGeolocation
    }
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
