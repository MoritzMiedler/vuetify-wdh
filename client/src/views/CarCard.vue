<template>
  <v-card>{{ cardata.id }}</v-card>
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
