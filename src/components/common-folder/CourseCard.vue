<template>
  <div class="card h-100">
    <img :src="courseKey.image" class="card-img-top" alt="SideView1" />
    <div class="card-body">
        <div>
        <div>
            <!-- <span class="badge bg-primary">{{ durations }}</span>
            <span class="badge bg-primary">Web Design</span> -->
        </div>
        </div>
      <h5 class="card-title">{{ courseKey.title }}</h5>
      <p class="card-text text-muted">
       {{ courseKey.description }}
      </p>
      <button class="btn-custom" @click="getCourse(courseKey.Id)">
        {{ courseKey.buttonText }}
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

defineProps({
 courseKey:{
    type: Object,
    required: true
 }
});

const emit = defineEmits(["Clicked"]);

const getCourse = (id) => {
  emit ("Clicked", `Child Card ${id} Says Hi`)
}


</script>

<style lang="scss" scoped></style>
