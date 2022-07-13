<template>
  <div class="mx-4 mt-10 d-flex justify-space-between align-center">
    <div>
      <h1>Dashboard</h1>
      <p>Here's Your analytical details</p>
    </div>
    <div class="d-flex align-center">
      <div class="date pa-2 mx-3">
        <v-icon>mdi-clock-time-eight-outline</v-icon> 20 Jan,2022-20 Feb,2022
        <v-icon>mdi-chevron-down</v-icon>
      </div>
      <div class="date pa-2">Funnel <v-icon>mdi-chevron-down</v-icon></div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.date {
  background-color: #f1f1f1;
  border-radius: 10px;
}
</style>
