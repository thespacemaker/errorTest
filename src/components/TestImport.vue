<script setup lang="ts">
const props = defineProps({
  title: { type: String, required: false },
  form: { type: Object, required: false },
})
</script>

<template>
  <h2>{{ props.title }}</h2>
  <component :is="props.form" v-if="props.form" />
</template>

