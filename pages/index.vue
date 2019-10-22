<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <signature/>
    </v-flex>
  </v-layout>
</template>

<script>
import Signature from '~/components/Signature.vue'

export default {
  components: {
    Signature
  }
}
</script>
