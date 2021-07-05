<template>
  <b-navbar fixed-top spaced class="navbar">
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <div class="logo">C</div>
      </b-navbar-item>
    </template>
    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <NuxtLink to="/" class="button is-rounded is-link is-inverted">
            Home
          </NuxtLink>
          <NuxtLink to="/contact" class="button is-rounded is-link is-inverted">
            Contact
          </NuxtLink>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
export default {}
</script>
