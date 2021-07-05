<template>
  <div>
    <footer class="footer has-text-centered">
      <NuxtLink to="/">
        <div class="logo">C</div>
      </NuxtLink>
      <div>
        <a
          href="https://www.linkedin.com/in/cokorda-agung-yudhana-505a9b66/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <font-awesome-icon :icon="['fab', 'linkedin']" class="network_icon" />
        </a>
        <a
          href="https://github.com/ckrdi"
          target="_blank"
          rel="noopener noreferrer"
        >
          <font-awesome-icon :icon="['fab', 'github']" class="network_icon" />
        </a>
        <a
          href="https://twitter.com/ckrdi"
          target="_blank"
          rel="noopener noreferrer"
        >
          <font-awesome-icon :icon="['fab', 'twitter']" class="network_icon" />
        </a>
      </div>
      <a href="https://bulma.io">
        <img
          src="https://versions.bulma.io/0.7.0/images/made-with-bulma.png"
          alt="Made with Bulma"
          width="128"
          height="24"
        />
      </a>
    </footer>
  </div>
</template>

<script>
export default {}
</script>
