<template>
  <div>
    <h1>Test</h1>
    <HelloWorld :greeting-message="greeting" />
    <button @click.prevent="onClickChange">change message</button>
  </div>
</template>

<script setup lang="ts">
  const greeting = ref<string>('i hacking with u')

  const onClickChange = () => {
    greeting.value = 'kamu berubahhh'
  }
</script>
