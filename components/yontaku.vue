<template>
  <div>
    <v-btn block rounded outlined>{{ texts[0] }}</v-btn>
    <v-btn block rounded outlined>{{ texts[1] }}</v-btn>
    <v-btn block rounded outlined>{{ texts[2] }}</v-btn>
    <v-btn block rounded outlined>{{ texts[3] }}</v-btn>
  </div>
</template>

<script>
export default {
  name: 'Yontaku',
  props: {
    texts: {
      type: Array,
      default: () => ["Nothing", "Nothing", "Nothing", "Nothing"]
    },
  }
}
</script>

<style scoped></style>