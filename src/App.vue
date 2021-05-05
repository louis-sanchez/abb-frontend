<template>
  <div id="app">
    <h2>ABB Frontend</h2>
    <control/>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return {
      connection: null,
      part: null
    };
  },
  methods: {
    sendMessage: function (message) {
      console.log(this.connection);
      this.connection.send(message);
    },
  },
  created: function () {
    
    console.log("Starting connection to WebSocket Server");
    this.connection = new WebSocket("ws://localhost:3000");

    this.connection.onopen = function (event) {
      console.log(event);
      console.log("Successfully connected to the echo websocket server...");
    };

    this.connection.onmessage = function ({ data }) {
      console.log(data)
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
