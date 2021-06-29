<template>
  <section class="section is-medium">
    <div class="container">
      <h1 class="title">My Projects</h1>
      <p class="subtitle">Collection of my recents personal projects.</p>
      <div class="columns is-desktop">
        <div v-for="card in 3" :key="card" class="column">
          <Card />
        </div>
      </div>
      <div class="columns is-desktop">
        <div v-for="card in 3" :key="card" class="column">
          <Card />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style></style>
