<script setup>
    import AcademicColumn from './Experience/AcademicColumn.vue';
    import ProfessionalColumn from './Experience/ProfessionalColumn.vue';
    import { onMounted } from "vue";
    import AOS from "aos";

    onMounted(() => {
    AOS.init();
})


</script>

<template>
    <section id="experience" class="pa-5">
        <div class="  flex items-center justify-center"  >
            <div class=" mx-4 p-4 text-center md:p-8" data-aos="fade-down">
              <h1 class="topic" 
              >Experience</h1>
              <p color="#666666" >Academic and Professional</p>
              <hr/>
            </div>
        </div>

        <div class="container-fluid flex flex-wrap row">
			<div class="w-full sm:w-6/12 mr-auto card-mobile left ">
				<AcademicColumn />
			</div>
            <div class="w-full sm:w-6/12 card-mobile right">
                <ProfessionalColumn />

            </div>
		</div>


    </section>
</template>

<style scoped>
*{
    color: wheat;
}
#experience{
    background-color: #353535;
}
.topic{
    font-size: 2.6rem;
    padding: 2px 10px;
    text-align: center;
    text-transform: uppercase;
}
hr {
    margin-top: 1em;
    border: 1px solid;
  }
  .row {
    padding-top: 20px;
    text-align: center;
  }
 

  @media (min-width:767px) {
    .left {
      text-align: right;
      border-right: 2px solid ;
      padding-right: 10px;
    }
    .right {
      text-align: left;
      padding-left: 10px;
    }
  }
  
  @media (max-width: 767px) {
    .right {
      margin-top: 20px;
      
    }
    .left:before {
      content : "";
      position: absolute;
      left    : 20%;
      bottom  : 0;
      height  : 2px;
      width   : 60%;  /* or 100px */
      

      
  }
  }
  
  
</style>