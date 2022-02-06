<template>
  <div>
    <div class="container">
      <a href="https://CapitalRoomate.net"><img class="logo" src="@/assets/logo.svg" alt="Logo"></a>

      <form @submit.prevent="handleSubmitForm">
        <div class="form-group">
          <label for="Bill">Bill:</label>

          <div class="form-group-inner">
            <input type="text" class="bill" placeholder="utility" required>
            <button class="add">Add</button>
          </div>
        </div>
      </form>

      <div class="bill-container">
        <div class="grid-item">
          <p class="billitem">Bill</p>
        </div>
        <div class="grid-item">
          <p class="price">Costs</p>
        </div>
        <div class="grid-item">
          <input type="text" class="person" placeholder="John" required>
        </div>
        <div class="grid-item">
          <button class="add-btn"><img src="@/assets/add.svg" alt="delete bill" width="25" height="25"></button>
        </div>
      </div>

      <div class="bill-container">
        <div class="grid-item">
          <p class="total">Total</p>
        </div>
        <div class="grid-item">
          <p class="totalcost">$0</p>
        </div>
        <div class="grid-item">
          <p class="personcost">$0</p>
        </div>
        <div class="grid-item">
          <button class="add-btn"><img src="@/assets/delete.svg" alt="delete bill" width="25" height="25"></button>
        </div>
      </div>

    </div>
  </div>
</template>

<script>

</script>

<style>
  * {
    box-sizing: border-box;
  }
  body {
    background: #24262A;
    color: white;
    margin: 0;
    font-family: 'Helvetica';
  }
   
  .logo {
    margin: 3em 0;

  }

  .container {
    text-align:center;
    margin: 0 1em;
  }

  .form-group {
    text-align: left;
    width: 300px;
    margin:7em auto;
  }

  label {
    font-weight: bold;
    margin-bottom: .7em;
    display: block;
  }

  .bill {
    padding: 1em;
    outline: none;
    border: none;
    border-top-left-radius: .3em;
    border-bottom-left-radius: .3em;
    font-size: 1.3em;
  }

  .form-group-inner {
    display: grid;
    grid-template-columns: 200px auto;
  }

  button.add {
    font-size: 1em;
    font-weight: bold;
    color: white;
    background: #856C81;
    border: none;
    outline: none;
    padding: 1em 3em;
    border-top-right-radius: .3em;
    border-bottom-right-radius: .3em;
  }

  .bill-container {
    display: grid;
    grid-template-columns: auto auto auto;
    background-color: gainsboro;
    padding: 10px
  }

  .grid-item {
    grid-row-start: 1;
    grid-row-end: 4;
    background-color: gainsboro;
    border: 1px solid black;
    text-align: center;
  }

  .add-btn {
    background: none;
    border: none;
    margin-top: 10px;
    cursor: pointer;
    outline: none;
  }

  .person {
    outline: none;
    border: none;
    margin-top: 12.5px;
    font-size: 1em;
  }


</style>
