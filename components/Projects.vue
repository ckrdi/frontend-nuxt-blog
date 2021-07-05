<template>
  <div class="projects">
    <div class="success"></div>
    <section class="section is-medium">
      <div class="container">
        <h2 class="main-title is-white">My Projects</h2>
        <p class="main-description is-white">
          Collection of my recents personal projects.
        </p>
        <div class="columns is-multiline">
          <div v-for="post in posts" :key="post.id" class="column is-one-third">
            <Card :posty="post" />
          </div>
        </div>
      </div>
      <a href="https://github.com/ckrdi">
        <button class="button is-rounded is-link is-outlined project-button">
          See more on Github
        </button>
      </a>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          id: '1',
          image: 'four-card-feature',
          link: 'https://ckrdi.github.io/four-card-feature/',
        },
        {
          id: '2',
          image: 'article-preview',
          link: 'https://ckrdi.github.io/article-preview-component/',
        },
        {
          id: '3',
          image: 'faq',
          link: 'https://ckrdi.github.io/faq-accordion-card/',
        },
        {
          id: '4',
          image: 'live-chatroom',
          link: 'https://vue-project-ed417.firebaseapp.com/',
        },
        {
          id: '5',
          image: 'share-playlist',
          link: 'https://vue-shareplaylist.firebaseapp.com/',
        },
        {
          id: '6',
          image: 'social-proof-section',
          link: 'https://ckrdi.github.io/social-proof-section/',
        },
      ],
    }
  },
}
</script>
