<template>
  <div>
    <h1>Hello {{ greetings }}</h1>
    <p>{{ greetingMessage }}</p>
  </div>
</template>

<script setup lang="ts">
  interface Props {
    greetings?: string
    // declare long prop menggunakan camelCase untuk menghindari tanda kutip saat menggunakannya sebagai property keys
    greetingMessage: string
  }

  const { greetings = 'guest' } = defineProps<Props>()
</script>
