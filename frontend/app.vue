<template>
  <div>
    <h2>{{ greetingText }}</h2>
  </div>
</template>

<script setup >
  const { find } = useStrapi();
  const greetingText = await find('hello');

</script>