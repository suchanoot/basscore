<template>
  <div id="app">
    <table class="show" border=0 cellspacing=0 width=400px height=150px style="margin-top:100px">
      <tr>
        <td>
            <h1 class="show">{{scoreLeft}} &nbsp&nbsp&nbsp<img src="http://www.clipartkid.com/images/70/the-totally-free-clip-art-blog-sports-basketball-with-hoop-sZvMsl-clipart.png" width="25%">&nbsp&nbsp&nbsp {{scoreRight}}</h1>
        </td>
     </tr>
   </table>
  </div>
</template>

<script>
export default {
  props: ['scoreLeft', 'scoreRight']
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

h1.show {
  font-size: 55px;
  color: #E6E6FA; text-shadow: black 0.1em 0.1em 0.2em
}

table.show {
  border-radius: 50px;
  background-color:#FDF5E6;
}
</style>
