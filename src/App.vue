<script setup>
import Banner from './components/Banner.vue';
import Footer from './components/Footer.vue';
import Gallery from './components/Gallery.vue';
import Header from './components/Header.vue';
import OurCourses from './components/OurCourses.vue';
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
}
.container{
    width: 100%;
    max-width: 1180px;
    margin: 0 auto;
    padding-left: 15px;
    padding-right: 15px;
    box-sizing: border-box;
}
</style>
