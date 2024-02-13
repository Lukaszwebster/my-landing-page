<script setup>
const projectOverviewItems = [
  {
    title: 'Social Seal landing page',
    subtitle: '',
    description: '',
    imgUrl: '',
    href: '',
    skills: [],
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
