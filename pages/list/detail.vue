<template>
  <h1>list-detail</h1>
  <TestView>{{ data }}</TestView>
</template>

<script setup lang="ts">
// const data = await $fetch('https://at.alicdn.com/t/c/font_4490668_5botfm3fkmc.js', { parseResponse: (txt) => txt })
const data = await useAsyncData(
  'mountains',
  () => $fetch('https://at.alicdn.com/t/c/font_4490668_5botfm3fkmc.js', { parseResponse: (txt) => txt })
)

</script>
