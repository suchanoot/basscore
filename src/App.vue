<template>
  <div id="app">

    <bas-header></bas-header>
    <show :score-left="scoreLeft" :score-right="scoreRight"></show>
    <bas-button :add-button-l1="AddButtonL1" :add-button-l2="AddButtonL2" :add-button-l3="AddButtonL3" :reduce-button-l="ReduceButtonL"
      :add-button-r1="AddButtonR1" :add-button-r2="AddButtonR2" :add-button-r3="AddButtonR3" :reduce-button-r="ReduceButtonR" :button-reset-l="ButtonResetL" :button-reset-r="ButtonResetR"
    ></bas-button>
  </div>
</template>
<script>
import BasHeader from './components/BasHeader.vue'
import show from './components/show.vue'
import BasButton from './components/BasButton.vue'

export default {
  data () {
    return {
      scoreLeft: 0,
      scoreRight: 0
    }
  },
  components: {
    BasHeader,
    show,
    BasButton
  },
  methods: {
    AddButtonL1: function () {
      this.scoreLeft++
    },
    AddButtonL2: function () {
      this.scoreLeft = this.scoreLeft + 2
    },
    AddButtonL3: function () {
      this.scoreLeft = this.scoreLeft + 3
    },
    ReduceButtonL: function () {
      this.scoreLeft --
      if (this.scoreLeft < 0) {
        this.scoreLeft = 0
      }
    },
    AddButtonR1: function () {
      this.scoreRight++
    },
    AddButtonR2: function () {
      this.scoreRight = this.scoreRight + 2
    },
    AddButtonR3: function () {
      this.scoreRight = this.scoreRight + 3
    },
    ReduceButtonR: function () {
      this.scoreRight --
      if (this.scoreRight < 0) {
        this.scoreRight = 0
      }
    },
    ButtonResetL () {
      this.scoreLeft = 0
    },
    ButtonResetR () {
      this.scoreRight = 0
    }
  }
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
</style>
