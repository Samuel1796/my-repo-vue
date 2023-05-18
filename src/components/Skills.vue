<script setup>
    import { onMounted } from "vue";
    import AOS from "aos";

    onMounted(() => {
    AOS.init();
})

</script>


<template>
    <section id="skills"  class="pa-5">
        <div class="  flex items-center justify-center"  >
            <div class=" mx-4 p-4 text-center md:p-8" data-aos="fade-down">
              <h1 class="topic" 
              >Skills</h1>
              <p color="#666666" >Abilities at a glance</p>
              <hr/>
            </div>
        </div>


        <div class="section-content">
            <div class="container-fluid">
                <div class="row d-flex flex-wrap align-items-center">
                    <div class="col-md-2 m-auto pb-0 test">
                            <img id="imgLogo" class="img-responsive mx-auto mt-3 " src="@/assets/logos/java.png" alt="Java" />
                            <div id="divAlt" class="altCaption text-center"> JAVA</div>
                    </div>
                    <div class="col-md-2 m-auto pb-0 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-3 " src="@/assets/logos/github.png" alt="Github" />
                        <div id="divAlt" class="altCaption text-center"> GITHUB</div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-7" src="@/assets/logos/vuejs.png" alt="Vue" />
                        <div id="divAlt" class="altCaption text-center"> VUE JS</div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-5" src="@/assets/logos/bootstrap.png" alt="Bootstrap" />
                        <div id="divAlt" class="altCaption text-center"> BOOTSTRAP </div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto " src="@/assets/logos/cplusplus.png" alt="C++" />
                        <div id="divAlt" class="altCaption text-center"> C++</div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-3" src="@/assets/logos/vuetify.png" alt="Vuetify" />
                        <div id="divAlt" class="altCaption text-center"> VUETIFY</div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-12" src="@/assets/logos/tailwind.png" alt="Tailwind" />
                        <div id="divAlt" class="altCaption text-center"> TAILWIND </div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-12" src="@/assets/logos/node.png" alt="NodeJs" />
                        <div id="divAlt" class="altCaption text-center"> NODE JS</div>
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-2 " src="@/assets/logos/html.png" alt="Html" />
                    </div>
                    <div class="col-md-2 m-auto pb-4 test">
                        <img id="imgLogo" class="img-responsive mx-auto mt-2 " src="@/assets/logos/css.png" alt="CSS" />
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<style scoped>
.test{
    height: 12em;
    width: 10em;
}

*{
    color: black;
}
#skills{
    background-color: wheat;
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


  @media(min-width: 992px) {
    .section-content {
        width: 80%;
        margin: 0 auto;
    }
}

img{
    max-width: 120px;
}

.altCaption{
    color: black;
    margin-top: 1rem;
    font-size: 1.5rem;
    padding-bottom: 0;
    text-align: center;

}
</style>