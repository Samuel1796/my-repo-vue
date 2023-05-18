<script setup>
    import s from '@/data/AcademicData.json'
    import {ref} from 'vue'
    
    const Academics = ref(s);


</script>

<template>
    <div>
        <h3 class="sub-topic"><strong>Academic</strong></h3>
        <div class="description"
        v-for="Academic in Academics"
        :key="Academic.id">

        <div class="date">{{Academic.date}}</div>
        <div class="topic"><strong>{{Academic.topic}}</strong></div>
        <div class="school">{{Academic.school}}</div>


        </div>
    </div>
</template>

<style scoped>
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
</style>