
<template>
  <v-footer
    contain
    color="lime darken-1"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <!-- <v-col
        class="primary lime darken-1 py-2 text-center white--text"
        cols="12"
      >
        {{ new Date().getFullYear() }} — <strong>Solgadie de papel</strong>
      </v-col> -->
    </v-row>
  </v-footer>
</template>

<script>
export default {
    name: 'Footer',
    data: () =>({
        links: [
            'Home',
            'Facebook',
            'Instagram'
        ]
    })
}
</script>