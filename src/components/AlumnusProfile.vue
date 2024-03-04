<template>
  <div class="">
    <h4>{{ alumnus.name }}</h4>
    <p>{{ alumnus.role }}</p>
    <div class="flex items-center gap-2">
        <a v-for="socialLink in alumnus.social" :href="socialLink.url" class="text-blue-500 text-base font-semibold">{{ socialLink.name }}</a>
    </div>
  </div>
</template>

<script setup lang="ts">
const props = defineProps(['alumnus'])

console.log(props)
</script>

<style scoped></style>
