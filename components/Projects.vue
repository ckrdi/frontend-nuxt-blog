<template>
  <div class="projects">
    <section class="success"></section>
    <section class="section is-medium">
      <div class="container">
        <h1 class="title">My Projects</h1>
        <p class="subtitle">Collection of my recents personal projects.</p>
        <div class="columns">
          <div v-for="card in 3" :key="card" class="column">
            <Card />
          </div>
        </div>
        <div class="columns">
          <div v-for="card in 3" :key="card" class="column">
            <Card />
          </div>
        </div>
      </div>
      <button class="button is-success">See more on Github</button>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.projects {
  position: relative;
}
.success {
  background-color: #48c78e;
  position: absolute;
  top: 0;
  height: 400px;
  width: 100%;
}
.title,
.subtitle {
  color: white;
}
.button {
  margin-top: 3rem;
}
</style>
