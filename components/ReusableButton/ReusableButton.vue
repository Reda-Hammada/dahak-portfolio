<template>
  <button :class="variant">{{ text }}</button>
</template>
<script setup lang="ts">
interface buttonTypes {
  text: string;
  variant: string;
}
const { variant, text } = defineProps<buttonTypes>();
</script>
