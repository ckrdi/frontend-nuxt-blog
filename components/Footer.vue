<template>
  <div class="main-footer">
    <div class="footer-back"></div>
    <footer class="footer has-text-centered">
      <div class="tile is-ancestor">
        <div class="tile is-parent">
          <div class="tile is-child notification is-link">
            <div class="columns is-vcentered">
              <div class="column is-8">
                <p class="main-title is-white">Do you want to ask something?</p>
              </div>
              <div class="column">
                <NuxtLink to="/contact">
                  <button class="button is-rounded is-link is-light">
                    Contact me
                  </button>
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="links">
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
