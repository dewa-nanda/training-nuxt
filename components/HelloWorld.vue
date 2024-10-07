<template>
  <div>
    <h1>Hello {{ props.greetings }}</h1>
    <p>It's single component</p>
  </div>
</template>

<script setup lang="ts">
  interface Props {
    greetings: string
  }

  const props = defineProps<Props>()
</script>
