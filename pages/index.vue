<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card>
        <v-card-title class="headline">
          Hi from Nuxt PWA
        </v-card-title>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  mounted(){
    this.$sentry.captureException(new Error('example'))
  }
}
</script>

<style scoped>
.headline {
  margin-top: 300px;
}
</style>
