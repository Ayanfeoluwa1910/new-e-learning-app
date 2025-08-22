<template>
  <div>
    <section class="about-container" container>
      <SectionContent
        :heading="content.title"
        :des="content.des"
        :btn="content.routeName"
        :btn2="content.routeName2"
      ></SectionContent>
    </section>
  </div>
</template>

<script setup>
import SectionContent from "@/components/common-folder/SectionContent.vue";

const content = {
  title: "About Section",
  des: `
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quia, voluptate vitae fugiat adipisci culpa ipsum repellendus, inventore, ratione reiciendis perspiciatis repudiandae aliquam deleniti similique suscipit velit doloremque odio unde magnam!
    `,
  routeName: "View Course",
  routeName2: "View More",
};
</script>

<style lang="scss" scoped></style>
