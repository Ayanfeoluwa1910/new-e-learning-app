<template>
  <header class="header-container">
    <div style="padding: 50px 16px 16px">
      <Announcement/>
      <Navbar/>
    </div>
  </header>
</template>

<script setup>
import Announcement from "../layout-folder/Announcement.vue";
import Navbar from "@/components/layout-folder/Navbar.vue";
</script>

<style lang="scss" scoped></style>
