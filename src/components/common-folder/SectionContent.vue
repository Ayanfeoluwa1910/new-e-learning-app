<template>
  <div class="content-section-container container row">
    <div class="content col-12 col-md-8">
      <h1 class="section-heading">{{ heading }}</h1>
      <p class="section-description text-dark">
       {{ des }}
      </p>
    </div>
    <div class="btn-container d-flex gap-3 mt-5 col-12 col-md-4 align-items-end justify-content-end">
      <button class="btn-custom" >{{ btn }}</button>
      <button class="btn-custom" v-if="btn2" >{{ btn2 }}</button>
    </div>
  </div>
</template>

<script setup>
defineProps({
    heading: String, 
    des: String,
    btn: String, 
    btn2: String,
})
</script>

<style lang="scss" scoped>

</style>
