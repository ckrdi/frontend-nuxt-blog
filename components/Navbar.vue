<template>
  <b-navbar fixed-top spaced>
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <strong>Cokorda Agung</strong>
      </b-navbar-item>
    </template>
    <template #end>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        Home
      </b-navbar-item>
      <b-navbar-item tag="router-link" :to="{ path: '/contact' }">
        Contact
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style></style>
