<script setup>
    import p from '@/data/ProfessionalData.json'

    import {ref} from 'vue'
    
    const Professionals = ref(p);

</script>

<template>
    <div>
        <h3 class="sub-topic"><strong>Professional</strong></h3>
        <div class="description"
        v-for="Professional in Professionals"
        :key="Professional.id">

        <div class="date">{{Professional.date}}</div>
        <div class="topic"><strong>{{Professional.topic}}</strong></div>
        <div class="school">{{Professional.school}}</div>
        <ul v-for="techs in Professional.tech" class="techs"
        :id="techs.id">
            <li>{{techs.lang}}</li>
        </ul>
        


        </div>

    </div>
</template>

<style scoped>

  ul li::before {
    content: "\2192"; /* Unicode character for right arrow */
    margin-right: 0.5em;
    display: inline-block;
    width: 1em;
  }
.sub-topic{
    font-size: 1.7rem;
    padding-bottom: 1.2em;
    text-transform: uppercase;
}
.description{
    margin-bottom: 25px;
}
.date {
    font-weight: 600;
    margin-bottom: 5px;
    color: rgb(248, 235, 209);

  }
  .topic {
    font-size: 1.3rem;
    color: wheat;
  }
  .school{
    color: rgb(248, 235, 209);
  }
  .techs{
    color: rgb(248, 235, 209);
    margin-left: 2em;
  }
</style>