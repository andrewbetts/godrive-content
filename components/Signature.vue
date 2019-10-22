<template>

    <v-card
      class="overflow-hidden mx-auto"
      height="100%"
      max-width="100%"
    >
      <v-simple-table>
        <template v-slot:default>
          <tbody>
            <tr>
              <td>Order number</td>
              <td>8687628374</td>
            </tr>
            <tr>
              <td>Date</td>
              <td>Wed, 16 Oct 12:10PM</td>
            </tr>
            <tr>
              <td>Address</td>
              <td>220 S 16th St., Philadelphia, PA 19102</td>
            </tr>                    
            <tr>
              <td>Phone number</td>
              <td>Contact customer</td>
            </tr>
            <tr>
              <td>Payment method</td>
              <td>Card</td>
            </tr>                    
          </tbody>
        </template>
      </v-simple-table>

      <v-bottom-navigation
        scroll-target="#scroll-area-2"
        hide-on-scroll
        scroll-threshold="500"
        absolute
        color="white"
        horizontal
      >
        <v-btn>
          <span>Notes</span>
          <v-icon>mdi-history</v-icon>
        </v-btn>

        <v-btn @click="showBlinkID()">
          <span>Signature</span>
          <v-icon>mdi-map-marker</v-icon>
        </v-btn>
      </v-bottom-navigation>

    </v-card>

</template>

<script>
  export default {
    name: 'Signature',
    data: () => ({
    }),
    methods: {
      showBlinkID () {
       showBlinkID.postMessage('')
        // alert('in showBlinkID');
      },      
    },
  }
</script>

<style>
.bottom-bar {
  background-color: "#00b3ee"
}

.theme--dark.v-application {
  background: "#ffffff"
}
</style>
