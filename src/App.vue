<template>
  <div id="app">
    <form
      id="myForm"
      method="post">

      <h2>Contact Us</h2>

      <label for="name">What's your name?</label>
      <span class="form-error">Please let us know what you call you by</span>
      <input
        type="text"
        name="name"
        placeholder="Your name"/>

      <label for="email">What's your email address?</label>
      <span class="form-error">Please provide a valid email address</span>
      <input
        type="text"
        name="email"
        placeholder="Your email address"/>

      <label for="phone">What's your phone number?</label>
      <span class="form-error">Please provide a valid phone number</span>
      <input
        type="tel"
        name="phone"
        placeholder="Your phone number"/>

      <span class="form-error">
        Please provide either an email address <strong>or</strong> phone number
      </span><br/>
      <span class="form-error">Please provide your name</span><br/>

      <button type="submit" class="button">Submit this form</button>

    </form>
  </div>
</template>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  padding: 1rem;
}

// override base Foundation styles
.form-error {
  display: inline-block;
}
</style>
