<script setup>
import GitHubCalendar from 'github-calendar'

const calendar = ref()
onMounted(() => {
  GitHubCalendar(calendar.value, 'Lukaszwebster', { responsive: true })
})
</script>

<template>
  <div>
    <h2 class="mx-4 mt-10 text-[1.5rem] lg:mx-[80px]">
      GitHub activity
    </h2>
    <div class="mx-4 mt-4 lg:mx-[100px] xl:mx-[300px]">
      <div ref="calendar" />
    </div>
  </div>
</template>
