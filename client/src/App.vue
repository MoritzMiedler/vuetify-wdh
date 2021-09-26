<template>
  <v-app>
    <v-main>
      <CarCards></CarCards>
    </v-main>
  </v-app>
</template>

<script>
import CarCards from '@/views/CarCards.vue';
export default {
  name: 'App',
  data: () => ({}),
  components: {
    CarCards,
  },
};
</script>
