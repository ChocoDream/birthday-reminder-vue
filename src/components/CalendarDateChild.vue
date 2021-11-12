<template>
  <div>
    <h3>Name: {{ name }}</h3>
    <h4>{{ date }}</h4>
  </div>
</template>

<script>
export default {
  props: {
    date: {
      type: String,
      required: true,
      default: "1970-01-01",
    },
    name: {
      type: String,
      required: true,
      default: () => {
        const random = Math.floor(Math.random() * 2);
        return random === 1 ? "Joan Doe" : "Jane Doe";
      },
    },
  },
};
</script>

<style></style>
