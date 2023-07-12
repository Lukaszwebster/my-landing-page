<script setup>
const props = defineProps({
  name: {
    type: String,
  },
  id: {
    type: Number,
  },
})
</script>

<template>
  <div class="m-4px inline-block rounded-4px bg-#fafafa px-2 py-1">
    {{ props.name }}
  </div>
</template>
