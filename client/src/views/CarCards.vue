<template>
  <div><CarCard v-for="(car, i) in cardata" :key="i"></CarCard></div>
</template>

<script>
import CarCard from '@/views/CarCard.vue';
import axios from 'axios';
export default {
  data() {
    return {
      cardata: [],
    };
  },
  components: {
    CarCard,
  },
  methods: {
    async getCars() {
      const cars = await axios({ method: 'GET', url: 'http://127.0.0.1:3000/cars' });

      this.cardata = cars.data;
    },
  },

  created() {
    this.getCars();
  },
};
</script>

<style lang="scss" scoped></style>
