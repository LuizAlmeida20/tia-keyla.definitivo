<template>
  <v-app>
    <web-site />
  </v-app>
</template>

<script lang="ts">
  import WebSite from "@/components/WebSite.vue";

  export default {
    data() {
      return {

      }
    },
    components: {
      WebSite
    }
  }
</script>

<style>
  * {
    background-color: white;
  }
</style>
