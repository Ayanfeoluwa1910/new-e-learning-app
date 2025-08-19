<template>
  <div class="announcement-container bg-primary">
    <p
      class="announcement-text d-flex justify-content-center align-items-center gap-3"
    >
      Free Courses 🌟 Sale Ends Soon, Get It Now
      <span><i class="fa-solid fa-arrow-right"></i></span>
    </p>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.announcement-container {
  border-radius: 8px;
}
  .announcement-text {
    padding: 10px 16px;
    font-size: 10px !important;

    // Small devices (landscape phones, 576px and up)
    @media (min-width: 400px) {
            font-size: 14px !important;
    }
}
</style>
