<template>
  <div>
    <section class="course-section">
      <SectionContent :heading="content.title" :des="content.des"  :btn="content.routeName" />
    </section>
  </div>
</template>

<script setup>
import SectionContent from "@/components/common-folder/SectionContent.vue";

const content = {
  title: "Course Section",
  des: `
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quia, voluptate vitae fugiat adipisci culpa ipsum repellendus, inventore, ratione reiciendis perspiciatis repudiandae aliquam deleniti similique suscipit velit doloremque odio unde magnam!
    `,
    routeName:"View Course"
};
</script>

<style lang="scss" scoped></style>
