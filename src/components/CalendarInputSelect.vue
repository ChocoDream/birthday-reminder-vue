<template>
  <select class="select">
    <option
      v-for="(option, i) of options"
      :key="`${option}+${i}`"
      :value="i"
    >
      {{ option }}
    </option>
  </select>
</template>

<script>
export default {
  props: {
    options: {
      required: true,
      type: Array,
    },
  },
  methods: {
    onSelect() {
      
    }
  }
};
</script>

<style scoped>
.select {
}
</style>
