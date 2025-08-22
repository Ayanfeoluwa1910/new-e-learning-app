<template>
  <section class="course-section">
    <SectionContent
      :heading="content.title"
      :des="content.des"
      :btn="content.routeName"
    />

    <!-- Course Card Container -->
    <div class="course-cards container mt-5">
      <div class="row g-4">
        <!-- Card 1 -->
        <div class="col-12 col-md-6 col-lg-4" v-for="course in courses" :key="course.id">
          <CourseCard  :courseKey="course" @Clicked="handleMessage"/>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import SectionContent from "../common-folder/SectionContent.vue";
import CourseCard from "../common-folder/CourseCard.vue";
import SideView1 from "../../assets/image/side-view-1.jpg";
import SideView2 from "../../assets/image/side-view-2.jpg";
import SideView3 from "../../assets/image/side-view-3.jpg";
import SideView4 from "../../assets/image/side-view-4.jpg";
import SideView5 from "../../assets/image/side-view-5.jpg";
import SideView6 from "../../assets/image/side-view-6.jpg";

const handleMessage = (message) => {
alert(message)
}

const content = {
  title: "Our Courses",
  des: `
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quia, voluptate vitae fugiat adipisci culpa ipsum repellendus, inventore, ratione reiciendis perspiciatis repudiandae aliquam deleniti similique suscipit velit doloremque odio unde magnam!
    `,
  routeName: "View Course",
};

const courses = [
  {
    id: 1,
    image: SideView1,
    duration: "4 Weeks",
    level: "Beginner",
    tutor: "John Smith",
    title: "Web Design Fundamentals",
    description:
      "Learn the fundamentals of web design, including HTML, CSS, and responsive design principles. Develop the skills to create visually appealing and user-friendly websites.",
    buttonText: "Get Web Development",
  },
  {
    id: 2,
    image: SideView2,
    duration: "6 Weeks",
    level: "Intermediate",
    tutor: "Jane Doe",
    title: "JavaScript Essentials",
    description:
      "Master the basics of JavaScript and learn how to make websites interactive. This course covers DOM manipulation, events, and modern ES6+ features.",
    buttonText: "Get JavaScript",
  },
  {
    id: 3,
    image: SideView3,
    duration: "8 Weeks",
    level: "Advanced",
    tutor: "Michael Lee",
    title: "React for Frontend Development",
    description:
      "Dive into React and build dynamic, scalable applications. Understand components, hooks, state management, and best practices in frontend development.",
    buttonText: "Get React",
  },
  {
    id: 4,
    image: SideView4,
    duration: "8 Weeks",
    level: "Advanced",
    tutor: "Michael Lee",
    title: "React for Frontend Development",
    description:
      "Dive into React and build dynamic, scalable applications. Understand components, hooks, state management, and best practices in frontend development.",
    buttonText: "Get Front-End",
  },
  {
    id: 5,
    image: SideView5,
    duration: "8 Weeks",
    level: "Advanced",
    tutor: "Michael Lee",
    title: "React for Frontend Development",
    description:
      "Dive into React and build dynamic, scalable applications. Understand components, hooks, state management, and best practices in frontend development.",
    buttonText: "Get Freelancing",
  },
  {
    id: 6,
    image: SideView6,
    duration: "8 Weeks",
    level: "Advanced",
    tutor: "Michael Lee",
    title: "React for Frontend Development",
    description:
      "Dive into React and build dynamic, scalable applications. Understand components, hooks, state management, and best practices in frontend development.",
    buttonText: "Get Data Science",
  },
];
</script>

<style lang="scss" scoped></style>
