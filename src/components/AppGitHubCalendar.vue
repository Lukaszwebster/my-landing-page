<script setup>
import GitHubCalendar from 'github-calendar'

const calendar = ref()
onMounted(() => {
  GitHubCalendar(calendar.value, 'Lukaszwebster', { responsive: true })
})
</script>

<template>
  <div ref="calendar" />
</template>
