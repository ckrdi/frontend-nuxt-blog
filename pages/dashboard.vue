<template>
  <section class="section">
    <div class="container" v-if="$auth.loggedIn">
      <h2 class="main-title">Dashboard</h2>
      <p class="main-description">Hi, {{ user.name }}</p>

      <button
        @click.prevent="logout"
        class="button is-rounded is-link is-inverted"
      >
        Logout
      </button>
    </div>
  </section>
</template>

<script>
export default {
  middleware: 'auth',
  data() {
    return {
      user: this.$auth.user,
    }
  },
  methods: {
    async logout() {
      await this.$auth.logout()
      this.$router.push('/login')
    },
  },
}
</script>

<style></style>
