<script setup>
  import Loader from '@/components/Loader.vue'
  import Main from '@/components/Main.vue'
  import About from '@/components/About.vue';
  import Experience from '@/components/Experience.vue';
  import Skills from '@/components/Skills.vue';
  import Projects from '@/components/Projects.vue';
  import Testimonials from '@/components/Testimonials.vue'
  import Footer from '@/components/constants/Footer.vue'
</script>


<template>
     <Loader/>
    <Main/>
    <About/>
    <Experience/>
    <Skills/>
    <Projects/>
    <Testimonials/>
    <Footer/>

</template>
 
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
*{
  font-family: 'Montserrat', sans-serif;}
  
</style>

