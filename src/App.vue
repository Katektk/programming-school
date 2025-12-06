<script setup>
import Banner from './components/Banner.vue';
import Footer from './components/Footer.vue';
import Gallery from './components/Gallery.vue';
import Header from './components/Header.vue';
import OurCourses from './components/OurCourses.vue';
import RoboticsСlub from './components/RoboticsСlub.vue';
import Robotics from './components/Robotics.vue';
import RunnigLine from './components/RunnigLine.vue';
import RunningLine2 from './components/RunningLine2.vue';
import Ticket from './components/Ticket.vue';
import Works from './components/Works.vue';
</script>

<template>
  <div class="container">
  <Header />
  <Banner />
  <RunnigLine />
  <OurCourses />
  <RoboticsСlub />
  <Robotics />
  <Works />
  <RunningLine2 />
  <Ticket />
  <Gallery />
  <Footer />

  </div>

</template>

<style>

body {
  font-family: 'Dela Gothic';
  background-color: white;
}
.container{
    width: 1200px;
    margin: 0 auto;
  
    align-items: center;
    justify-content: space-between;
}
</style>
