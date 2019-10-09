<template>
<div class="container" style="margin: 0 auto;">
     <v-card
    class="mx-auto"
    max-width="344"
  >
    <v-img
      src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
      height="200px"
    ></v-img>

    <v-card-title>
      <div>Grant Shoop</div>
      <span class="grey--text subtitle-1">Web Developer</span>
    </v-card-title>

    <v-card-actions>
      <v-btn text>Share</v-btn>

      <v-btn
        text
        color="purple"
      >
        Explore
      </v-btn>

      <div class="flex-grow-1"></div>

      <v-btn
        icon
        @click="show = !show"
      >
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-card-text>
         Lives in Pleasant Grove, Utah. Married and has one son. Likes to code and play video games.
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>


</div>
</template>

<script>
export default {
    
}
</script>




<style scoped>

</style>