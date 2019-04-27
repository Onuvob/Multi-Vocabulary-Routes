<template>
  <div id="app">
    <Header/>
    <div id="nav" class="text-center text-white">
      <router-link to="/">Home</router-link> | 
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'app',
  
  components: {
    Header
  },
  

}
</script>


<style>
#app {

  padding: 0;
  margin: 0;
  width: 100%;
  min-height: 100vh;
  
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background: linear-gradient(270deg, #246655, #194e81, #062734);
  background-size: 600% 600%;

  -webkit-animation: DynamicColorChanging 12s ease infinite;
  -moz-animation: DynamicColorChanging 12s ease infinite;
  animation: DynamicColorChanging 12s ease infinite;

  @-webkit-keyframes DynamicColorChanging {
      0%{background-position:0% 50%}
      50%{background-position:100% 50%}
      100%{background-position:0% 50%}
  }
  @-moz-keyframes DynamicColorChanging {
      0%{background-position:0% 50%}
      50%{background-position:100% 50%}
      100%{background-position:0% 50%}
  }
  @keyframes DynamicColorChanging {
      0%{background-position:0% 50%}
      50%{background-position:100% 50%}
      100%{background-position:0% 50%}
  }
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #ffcccc;
}

#nav a.router-link-exact-active {
  color: #ff3333;
}

</style>
