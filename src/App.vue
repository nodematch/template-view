<template>
  <header-navbar />
  <router-view />
</template>

<script lang="ts">
import { defineComponent } from "vue";
// import HeaderComponent from "@/components/HeaderComponent.vue";
import HeaderNavbar from "@/components/HeaderNavbar.vue";

export default defineComponent({
  components: {
    // HeaderComponent,
    HeaderNavbar,
  },
});
</script>

<style>
@import "../src/assets/css/color.css";
</style>
