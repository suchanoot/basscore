<template>
  <div id="app">
    <table border=0 cellspacing=0 width=400px height=150px style="margin-top:100px">
      <tr>
        <td>
    <button @click="AddButtonL1" >+1</button>
    <button @click="AddButtonL2" >+2</button>
    <button @click="AddButtonL3" >+3</button>
    <button @click="ReduceButtonL"  class="reduce">-1</button>
    <br><br><button @click="ButtonResetL" class="reset">reset</button>
        </td>

        <td>
    <button @click="AddButtonR1">+1</button>
    <button @click="AddButtonR2">+2</button>
    <button @click="AddButtonR3">+3</button>
    <button @click="ReduceButtonR" class="reduce">-1</button>
    <br><br><button @click="ButtonResetR" class="reset">reset</button>
        </td>
      </tr>
    </table>
  </div>
</template>
<script>
export default {
  props: ['AddButtonL1', 'AddButtonL2', 'AddButtonL3', 'ReduceButtonL', 'AddButtonR1', 'AddButtonR2', 'AddButtonR3', 'ReduceButtonR', 'ButtonResetL', 'ButtonResetR'],
  data () {
    return {
    }
  },
  components: {

  }
}
</script>

<style>
html {
  height: 100%;
}

button {
  height: 25%;
  width: 20%;
}

button {
    background-color:#FF69B4;
    cursor: pointer;
}

button.reduce:hover{
  background-color:#FF3333;
  cursor: pointer;
}

button:hover {
    background-color:#FFC0CB;
    box-shadow: 0 10px 15px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19);
    cursor: pointer;
}

button.reset {
  background-color: white;
  height: 17%;
  width: 25%;
  align-items: center;
  border-radius: 20px;
  color: black;
  border: 2px solid #4CAF50;
  cursor: pointer;
}

button.reset:hover {
  background-color: #4CAF50;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#app {
  color: #2c3e50;
  margin-top: -100px;
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
