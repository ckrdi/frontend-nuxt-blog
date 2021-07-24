<template>
  <section class="section">
    <div class="container">
      <div class="columns is-centered">
        <div class="column is-one-third">
          <h2 class="main-title has-text-centered">Login</h2>
          <form method="post" @submit.prevent="login">
            <div class="field">
              <label for="email" class="label">Email</label>
              <div class="control">
                <input type="email" class="input" v-model="email" />
              </div>
            </div>

            <div class="field">
              <label for="password" class="label">Password</label>
              <div class="control">
                <input type="password" class="input" v-model="password" />
              </div>
            </div>

            <div class="control">
              <button
                type="submit"
                class="button is-rounded is-link is-inverted"
              >
                Login
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  middleware: ['guest'],
  data() {
    return {
      email: '',
      password: '',
    }
  },
  methods: {
    async login() {
      await this.$auth.loginWith('laravelSanctum', {
        data: {
          email: this.email,
          password: this.password,
        },
      })
      this.$router.push('/dashboard')
    },
  },
}
</script>

<style></style>
