<template>
  <v-app>
    <web-site v-if="windowWidth > 835"/>
    <MobileSite v-if="windowWidth < 835"/>
  </v-app>
</template>

<script lang="ts">
  import WebSite from "@/components/WebSite.vue";
  import MobileSite from "@/components/MobileSite.vue";

  export default {
    data() {
      return {
        windowWidth: window.innerWidth as number
      }
    },
    components: {
      WebSite,
      MobileSite
    }
  }
</script>

<style>
  * {
    background-color: white;
  }
</style>
