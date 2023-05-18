<script setup>
 import { onMounted } from "vue";
import AOS from "aos";

onMounted(() => {
    AOS.init();
})


</script>

<template>
  <header class="bg-header flex items-center justify-center h-screen">
  <div class="  mx-4 p-4 text-center md:p-8">
    <h1 class="name" >Boakye Oduro Samuel</h1>
    <hr/>
    <p class="title">FullStack Developer</p>
  </div>
</header>


</template>


<style scoped>

  .bg-header {
  background: url(../assets/bgg.jpg);
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100%;
}

  .name {
    font-size: 2.3rem;
    padding: 2px 10px;
    text-align: center;
    text-transform: uppercase;
    color: wheat;
  }

  .title{
    font-size: 1.5rem;
    text-align: center;
    margin: 5px auto;
    color: wheat;
  }

  hr {
    margin-top: 2em;
    border: 1px solid wheat;
  }
</style>