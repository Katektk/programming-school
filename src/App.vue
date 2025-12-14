<script setup>
import Header from './components/Header.vue';
import Banner from './components/Banner.vue';
import OurCourses from './components/OurCourses.vue';
import Footer from './components/Footer.vue';
import Gallery from './components/Gallery.vue';
import RoboticsСlub from './components/RoboticsClub.vue';
import RunnigLine from './components/RunnigLine.vue';
import RunningLine2 from './components/RunningLine2.vue';
import Ticket from './components/Ticket.vue';
import Works from './components/Works.vue';
</script>

<template>
  <Header />
  <Banner />
  <RunnigLine />
  <OurCourses />
  <RoboticsСlub />
  <Works />
  <RunningLine2 />
  <Ticket />
  <Gallery />
  <Footer />
</template>

<style>

body {
  font-family: 'Marmelad';
  background-color: white;
  margin: 0;
}
.container {
max-width: 1290px;
margin: 0 auto;
}

</style>
