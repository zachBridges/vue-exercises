<template>
  <div>
    <h2>Update Your Email Address</h2>
    <p>Hi, {{%%firstName%%}}. Has your email recently changed? Update us if it has!</p>
    {{user}}
    <form v-on:submit.prevent="submitForm">
      <label for="emailAddress">
        Email Address</label>
      <span class="error" v-if="isFormInvalid">Please enter a valid email address</span>
      <input
        type="text"
        name="emailAddress"
        v-model="emailAddress"
        :placeholder="%%email%%"/>

      <button class="button">Update Email</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'EmailUpdate',
  data() {
    return {
      emailAddress: %%emailAddress%%,
      isFormInvalid: false,
    };
  },
  methods: {
    submitForm() {
      if (!this.emailAddress) {
        this.isFormInvalid = true;
        return;
      }
      // TODO: tell the parent component that the email address has been updated
    },
  },
};
</script>

<style lang="scss">
.error{color: red;}
label{
  font-weight: bold;
  text-align: left;
}
</style>

