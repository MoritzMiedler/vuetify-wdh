<template>
  <v-card>
    <v-img :src="cardata.image"></v-img>
    <span class="text-h5">{{ cardata.title }}</span>
    <br />
    <div>
      {{ cardata.owner.firstName }} {{ cardata.owner.lastName }}
      <br />
      {{ cardata.yearOfMake }}
      <br />
      {{ cardata.miles }}
      <br />
      {{ cardata.price }}
      <br />
      {{ cardata.description }}
    </div>
  </v-card>
</template>

<script>
export default {
  props: {
    cardata: {
      type: Array,
      default: () => {},
    },
  },
};
</script>

<style lang="scss" scoped></style>
