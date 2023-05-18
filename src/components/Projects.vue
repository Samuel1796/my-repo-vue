<script setup>
    import { onMounted } from "vue";
    import AOS from "aos";

    onMounted(() => {
    AOS.init();
})

import { reactive } from 'vue';
const items = reactive([
      {
        color: 'red-lighten-2',
        icon: 'mdi-star',
      },
      {
        color: 'purple-lighten-2',
        icon: 'mdi-book-variant',
      },
      {
        color: 'green-lighten-1',
        icon: 'mdi-airballoon',
      },
      {
        color: 'indigo-lighten-2',
        icon: 'mdi-layers-triple',
      },
    ]);

</script>


<template>
    
    <section id="projects" class="px-5">
        <div class="  flex items-center justify-center"  >
            <div class=" mx-4 p-4 text-center md:p-8" data-aos="fade-down">
              <h1 class="topic" 
              >My Projects</h1>
              <p color="#666666" >Featured works and collaborations</p>
              <hr/>
            </div>
        </div>


       <div class="timeline-container"> 
            <ol class="relative border-l border-gray-200 dark:border-gray-700">  
                                <!-- TRAVELS -->
                <li class="mb-10 ml-6">            
                    <span class="absolute flex items-center justify-center w-6 h-6 bg-blue rounded-full -left-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue">
                        <svg aria-hidden="true" class="w-3 h-3 text-blue-800 dark:text-blue-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
                    </span>
                    <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900 dark:text-white"><button type="button" class="text-white bg-gradient-to-br from-green-400 to-blue-600 hover:bg-gradient-to-bl focus:ring-4 focus:outline-none focus:ring-green-200 dark:focus:ring-green-800 font-medium rounded-lg text-sm px-2 py-1 text-center mr-2 mb-2">Vue.Js | Vuetify | Flowbite</button>
                        <span class="bg-blue text-blue-800 text-sm font-medium mr-2 px-2.5 py-0.5 rounded dark:bg-blue-900 dark:text-blue-300 ml-3">Latest</span></h3>
                    <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on May 1st, 2023</time>
                    <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
                        The UI of a platform where people book places for vacation . Here, we can share visit interesting places, bond with our loved ones and connect with local dwellers. 
                        <strong>Site Development is still in progress</strong></p>
                    
                    <img data-aos="fade-up-right" class="h-400 max-w-full" src="@/assets/projects/tinch.jpg" alt="image description">
                    
                    <p class="text-gray-500 dark:text-gray-400 mt-7">LINK:  <a href="https://vue-travels2.vercel.app" target="__blank" class="text-white inline-flex items-center font-medium text-blue-600 dark:text-blue-500 hover:underline">
                        Tinch Travels
                        <svg aria-hidden="true" class="w-5 h-5 ml-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                        </a></p>
    
                </li>

                <!-- NOTES -->
                <li class="mb-10 ml-6">            
                    <span class="absolute flex items-center justify-center w-6 h-6 bg-purple rounded-full -left-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue">
                        <svg aria-hidden="true" class="w-3 h-3 text-blue-800 dark:text-blue-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
                    </span>
                    <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900 dark:text-white"><button type="button" class="text-white bg-gradient-to-br from-purple-600 to-blue-500 hover:bg-gradient-to-bl focus:ring-4 focus:outline-none focus:ring-blue-300 dark:focus:ring-blue-800 font-medium rounded-lg text-sm px-2 py-1 text-center mr-2 mb-2">Vue.Js | CSS</button>
                        </h3>
                    <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on March 6th, 2023</time>
                    <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
                        Let's-Write is a simple website where uses can keep notes and write memos. 
                        <strong>The site now saves data in a from of JSON. Improvements will be made soon</strong></p>
                    
                    <img data-aos="fade-up-right" class="h-400 max-w-full" src="@/assets/projects/notes.jpg" alt="image description">
                    
                    <p class="text-gray-500 dark:text-gray-400 mt-7">LINK:  <a href="https://vue-travels2.vercel.app" target="__blank" class="text-white inline-flex items-center font-medium text-blue-600 dark:text-blue-500 hover:underline">
                        We-Write
                        <svg aria-hidden="true" class="w-5 h-5 ml-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                        </a></p>
    
                </li>

                <!-- JAVA -->
                <li class="mb-10 ml-6">            
                    <span class="absolute flex items-center justify-center w-6 h-6 bg-pink rounded-full -left-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue">
                        <svg aria-hidden="true" class="w-3 h-3 text-blue-800 dark:text-blue-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
                    </span>
                    <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900 dark:text-white"><button type="button" class="text-white bg-gradient-to-r from-purple-500 to-pink-500 hover:bg-gradient-to-l focus:ring-4 focus:outline-none focus:ring-purple-200 dark:focus:ring-purple-800 font-medium rounded-lg text-sm px-2 py-1 text-center mr-2 mb-2">Java | JavaFX</button>
                        </h3>
                    <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on February 14th, 2023</time>
                    <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
                        This is a mini java project which collect students details during based on the course he/she is offering and saves it in a .txt file
                        <strong>The GUI was made with JavaFX</strong></p>
                    
                    <img data-aos="fade-up-right" class="h-400 max-w-full" src="@/assets/projects/java.jpg" alt="image description">
                    
                    <p class="text-gray-500 dark:text-gray-400 mt-7">LINK:  <a href="#" target="__blank" class="text-white inline-flex items-center font-medium text-blue-600 dark:text-blue-500 hover:underline">
                        Java
                        <svg aria-hidden="true" class="w-5 h-5 ml-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                        </a></p>
    
                </li>
            </ol>

        </div>
    </section>
</template>

<style scoped>
    *{
        color: wheat;
    }
    #projects{
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

      .timeline-container {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 2em;
      }

      @media (min-width:767px) {
        .timeline-container{
            padding: 2em 20em;
        }

      }

      
      
</style>