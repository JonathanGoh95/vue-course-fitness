<script setup>
  import Welcome from './components/Pages/Welcome.vue'
  import Layout from './components/Layouts/Layout.vue'
  import Dashboard from './components/Pages/Dashboard.vue'
  import Workout from './components/Pages/Workout.vue'

  const selectedDisplay = 2
</script>

<template>
  <Layout>
    <!-- PAGE 1 -->
    <Welcome v-if = "selectedDisplay == 1"/>
    <!-- PAGE 2 -->
    <Dashboard v-if = "selectedDisplay == 2"/>
    <!-- PAGE 3 -->
    <Workout v-if = "selectedDisplay == 3"/>
  </Layout>
</template>

<style scoped>

</style>
