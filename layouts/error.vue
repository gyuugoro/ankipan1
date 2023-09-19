<template>
  <v-app>
    <v-app-bar app>
    </v-app-bar>

    <v-main>

      <v-container fluid>

        <v-btn to="/">ホームに戻る</v-btn>
      </v-container>
    </v-main>

  </v-app>
</template>

<script>
export default {
  name: 'EmptyLayout',
  layout: 'empty',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  data() {
    return {
      pageNotFound: '404 Not Found',
      otherError: 'An error occurred'
    }
  },
  head() {
    const title =
      this.error.statusCode === 404 ? this.pageNotFound : this.otherError
    return {
      title
    }
  }
}
</script>

<style scoped></style>
