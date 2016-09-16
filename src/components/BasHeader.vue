<template>
  <div id="app">
    <table border=0 cellspacing=0 width=400px height=80px style="margin-top:200px">
      <tr>
        <td>
          <h2>Basketball Score</h2>
          <h1>Home &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp  away</h1>
        </td>
     </tr>
   </table>
  </div>
</template>

<script>
export default {
}
</script>

<style>
html {
  height: 100%;
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

h2 {
  color: #2F4F4F;
  text-shadow: 0.1em 0.1em 0.3em black;
  font-size: 35px;
}
</style>
