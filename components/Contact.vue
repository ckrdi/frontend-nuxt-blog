<template>
  <div class="section">
    <div class="field">
      <label class="label">Name</label>
      <div class="control">
        <input class="input" type="text" placeholder="Your name" />
      </div>
    </div>

    <div class="field">
      <label class="label">Email</label>
      <div class="control">
        <input class="input" type="email" placeholder="Your email" />
      </div>
    </div>

    <div class="field">
      <label class="label">Subject</label>
      <div class="control">
        <input class="input" type="text" placeholder="Subject" />
      </div>
    </div>

    <div class="field">
      <label class="label">Message</label>
      <div class="control">
        <textarea class="textarea" placeholder="Your message"></textarea>
      </div>
    </div>

    <div class="field is-grouped">
      <div class="control">
        <button class="button is-rounded is-link is-inverted">Submit</button>
      </div>
      <div class="control">
        <button class="button is-rounded is-link is-inverted">Cancel</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
