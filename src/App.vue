<template>
  <div id="app">
    <h2>Mortgage Calculator</h2>
    <form>
      <label for="rate">Interest Rate</label>
      <input name="rate" type="number" placeholder="Interest Rate"/>
      <label for="term">Term (in months)</label>
      <input name="term" type="number" placeholder="Term (in months)"/>
      <label for="mortgage">Mortgage Amount</label>
      <input name="mortgage" type="number" placeholder="Mortgage Amount"/>
    </form>

    <table>
      <tbody>
        <tr>
          <td>Your monthly payment is: </td>
          <td>$<!-- payment amount--></td>
        </tr>
        <tr>
          <td>Total mortgage cost: </td>
          <td>$<!-- total mortgage --></td>
        </tr>
      </tbody>
    </table>


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
</style>
