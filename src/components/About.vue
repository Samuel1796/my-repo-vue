<script setup>


  import { onMounted } from "vue";
  import AOS from "aos";
  import Socials from '@/components/constants/Socials.vue'

onMounted(() => {
    AOS.init();
})



</script>

<template>
        <div class="  flex items-center justify-center"  >
            <div class=" mx-4 p-4 text-center md:p-8" data-aos="fade-down">
              <h1 class="topic" 
              >About Me</h1>
              <p color="#666666">Discover my story</p>
              <hr/>
            </div>
        </div>
<!-- IMAGE -->
        <div class="flex items-center justify-center me" >
            <img src="../assets/meeee.jpg" alt="My Photo">
     </div>

<!-- DESC -->
<div class="flex flex-wrap p-5 pl-10" >
  <div class="w-full sm:w-7/12 mr-auto card-mobile " data-aos="zoom-in">
    <h3 class="sub-topic pt-3">Who am i?</h3>
    <div class="mb-7 test text-left"><span class="main-text" >
      I am a motivated and ambitious individual, currently pursuing a degree in Computer Science and Engineering at the University of Mines and Technology.
       As a second-year student, I have already established myself as a full stack developer with a passion for programming and IoT projects. 
      My enthusiasm for technology extends beyond the classroom,
       as I actively engage with various online communities and leverage social media platforms to stay updated on the latest trends.
      </span><br/>
      <br/>

        I possess a high level of dedication and a natural ability to inspire others, 
        allowing me to make a positive impact wherever I go. 
        The satisfaction of solving complex problems has fueled my desire to continuously grow and excel in the field of technology.
  </div>
  </div>



  <div class="w-full sm:w-4/12 card-mobile" >
   <div class="test" data-aos="zoom-in">
    <h3 class="sub-topic">Boakye O. Samuel</h3>
    <div class="data"><strong>E-mail:</strong> sboakye1796@gmail.com </div>
    <div class="data"><strong>Phone: </strong> +233557272539</div>
    <div class="data"><strong>City: </strong> Sekondi-Takoradi, Ghana</div>
    <div class="data"><strong>Languages: </strong> French, English</div>



    <p class="font-general-semibold text-3xl sm:text-4xl pt-3">
    Follow me
  </p>
  <Socials/>
    
  </div>

  </div>
</div>



</template>



<style scoped>
*{
  background-color: wheat;
}
.main-text{
  color: #666666;
}
.topic{
    font-size: 2.6rem;
    padding: 2px 10px;
    text-align: center;
    text-transform: uppercase;
}
.sub-topic{
    font-size: 2rem;
    padding-bottom: 1.2em;
    text-align: center;

    text-transform: uppercase;
}
hr {
    margin-top: 1em;
    border: 1px solid black;
  }
.me img {
    width: fit-content;
    height: 420px;
    border-radius: 50%;
    display: inline-block;
}
.data {
  margin-bottom: 15px;
  color: #666666;
}

</style>