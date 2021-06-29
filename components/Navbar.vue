<template>
  <b-navbar fixed-top spaced>
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <strong>Cokorda Agung</strong>
      </b-navbar-item>
    </template>
    <template #end>
      <b-navbar-item href="#"> Home </b-navbar-item>
      <b-navbar-item href="#"> Projects </b-navbar-item>
      <b-navbar-item href="#"> Contact </b-navbar-item>
      <b-navbar-item href="#"> Blog </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
export default {}
</script>

<style></style>
