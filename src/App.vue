<template>
  <div id="app">
    <ourNavbar></ourNavbar>
    <ourContent class="content"></ourContent>
    <ourFooter></ourFooter>
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Content from "./components/Content";
import Footer from "./components/Footer";
export default {
  components: {
    ourNavbar: Navbar,
    ourContent: Content,
    ourFooter: Footer
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Arimo&display=swap");
body {
  margin: 0;
  padding: 0;
  background-color: white;
  color: #5b5a5a;
  background: url("./assets/corona.svg");
  background-repeat: no-repeat;
  background-size: 50% 50%;
  background-position: 140% -40%;
}
body::-webkit-scrollbar {
  width: 0.25rem;
}
body::-webkit-scrollbar-track {
  background: #5b5a5a;
}
body::-webkit-scrollbar-thumb {
  background: #c7d40f;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
}
:root {
  font-size: 16px;
}
.content {
  padding-top: 1rem;
  min-height: 100vh;
}
@media only screen and (max-width: 600px) {
  .content {
    margin: 0 0 4rem 0;
  }
}
@media only screen and (min-width: 600px) {
  .content {
    margin-left: 5rem;
  }
}
</style>
