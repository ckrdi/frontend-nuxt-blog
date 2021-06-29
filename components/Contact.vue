<template>
  <section>
    <b-field label="Name" :label-position="labelPosition">
      <b-input></b-input>
    </b-field>

    <b-field label="Email" :label-position="labelPosition">
      <b-input type="email"> </b-input>
    </b-field>

    <b-field label="Subject" :label-position="labelPosition">
      <b-input> </b-input>
    </b-field>

    <b-field label="Message" :label-position="labelPosition">
      <b-input type="textarea"></b-input>
    </b-field>

    <b-field
      ><!-- Label left empty for spacing -->
      <p class="control">
        <b-button label="Send message" type="is-success" />
      </p>
    </b-field>
  </section>
</template>

<script>
export default {
  data() {
    return {
      labelPosition: 'on-border',
    }
  },
}
</script>
