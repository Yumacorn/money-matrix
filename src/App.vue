<template>
  <img class="tinypic" alt="Piggy Bank" src="./assets/piggy-bank.jpg">
  <NavBar v-on:click="handleClick" />
  <div class="about-desc">
    <h1>About</h1>
    <p>
      <b>Money</b> can be a <b>source of anxiety and stress</b> for us.
    </p>
    <p>
      In order to <b>help relieve</b> some of those negative feelings,<br>
      here are some <b>easy and accessible tools</b> to <b>introduce, explore, and plan</b> for your finances.
    </p>
  </div>
  <FooterBar />
</template>

<script>
import NavBar from './components/Navbar.vue'
import FooterBar from './components/FooterBar.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    FooterBar
  },
  methods: {
    handleClick() {
      console.log('Button clicked!');
    }
  }
}
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

  .tinypic {
    width: 20%;
    height: 20%;
    border-color: black;
    border-style: double;
    align-items: center;
  }

  .about-desc {
    margin: auto;
    width: 60vw;
    font-size: large;
  }
  
  .about-desc b {
    color: blue;
    font-size: x-large;
  }

  button {
    border-radius: 20%;
    background-color: azure;
    font-size: large;
  }
</style>
