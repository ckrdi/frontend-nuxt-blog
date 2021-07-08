<template>
  <div class="section">
    <form @submit="handleSubmit">
      <div class="field">
        <label class="label" for="name">Name</label>
        <div class="control">
          <input
            class="input"
            name="name"
            type="text"
            placeholder="Your name"
            v-model="newMessage.name"
            required
          />
        </div>
      </div>

      <div class="field">
        <label class="label" for="email">Email</label>
        <div class="control">
          <input
            class="input"
            name="email"
            type="email"
            placeholder="Your email"
            v-model="newMessage.email"
            required
          />
        </div>
      </div>

      <div class="field">
        <label class="label" for="subject">Subject</label>
        <div class="control">
          <input
            class="input"
            name="subject"
            type="text"
            placeholder="Subject"
            v-model="newMessage.subject"
            required
          />
        </div>
      </div>

      <div class="field">
        <label class="label" for="message">Message</label>
        <div class="control">
          <textarea
            class="textarea"
            name="message"
            placeholder="Your message"
            v-model="newMessage.message"
            required
          ></textarea>
        </div>
      </div>

      <div class="field is-grouped">
        <div class="control">
          <button class="button is-rounded is-link is-inverted">Submit</button>
        </div>
        <div class="control">
          <button
            class="button is-rounded is-link is-inverted"
            @click="handleDeleteMessage"
          >
            Cancel
          </button>
        </div>
      </div>
      <div v-if="error">
        {{ error }}
      </div>
    </form>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  data() {
    return {
      newMessage: {
        name: '',
        email: '',
        subject: '',
        message: '',
      },
      error: null,
    }
  },
  methods: {
    handleDeleteMessage: function () {
      this.newMessage.name = ''
      this.newMessage.email = ''
      this.newMessage.subject = ''
      this.newMessage.message = ''
    },

    handleSubmit: async function (e) {
      this.error = null
      e.preventDefault()

      try {
        const response = await axios.post(
          'https://desolate-mountain-91022.herokuapp.com/messages',
          this.newMessage
        )
        this.newMessage.name = ''
        this.newMessage.email = ''
        this.newMessage.subject = ''
        this.newMessage.message = ''
        // console.log(response)
      } catch (error) {
        this.error = error
      }
    },
  },
}
</script>
