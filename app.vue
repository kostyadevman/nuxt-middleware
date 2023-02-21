<template>
  <div>
    <h2>{{  greetingText  }}</h2>
  </div>
</template>

<script setup lang="ts">
  const { data: greetingText } = await useFetch('/api/greeting')
</script>