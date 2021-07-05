<template>
  <div class="card" v-if="posty">
    <a :href="posty.link">
      <div class="card-image">
        <figure class="image">
          <img
            :src="require(`~/assets/images/${posty.image}.png`)"
            alt="website image"
          />
        </figure>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  props: {
    posty: Object,
  },
}
</script>
