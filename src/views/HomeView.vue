<template>
  <main class="font-inter bg-graditent-to-tr">
    <section class="mx-auto w-full max-w-[1440px] px-4 sm:px-6 md:px-8">
      <div class="grid grid-cols-4">
        <AlumnusProfile v-for="alumnus in alumniDB.alumni" :key="alumnus.id" :alumnus="alumnus" />
      </div>
    </section>
  </main>
</template>

<script setup lang="ts">
import alumniDB from '../db/alumniDB.json'

import AlumnusProfile from '../components/AlumnusProfile.vue'
</script>
