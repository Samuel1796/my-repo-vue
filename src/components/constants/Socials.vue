<script setup>

import s from '@/data/SocialHandles.json'
  import { ref } from 'vue';

  const socials = ref(s)
</script>

<template>
    <ul
     class="flex gap-4 sm:gap-8">
      <a
            v-for="social in socials"
						:key="social.id"
						:href="social.url"
        target="__blank"
        class="text-gray-400  cursor-pointer rounded-lg  p-4 "
        >
        <i
          class="w-5 sm:w-15 h-5 sm:h-15"
        > <img :src="social.icon" alt=""></i>
      </a>
      
    </ul>

</template>

<style scoped>
*{
  background-color: wheat;
}
a:hover{
  border: 2px solid black;
}
</style>