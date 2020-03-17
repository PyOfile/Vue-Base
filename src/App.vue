<template>
  <div id="app">
    <div id="nav">
      <b-navbar-brand href="/" class="mudblood">
        <img alt="Vue logo" src="./assets/images/artb1.png" class="d-inline-block align-top">
      </b-navbar-brand>
      <b-dropdown id="dropdown-right" size="lg" right text="☰" variant="secondary" class="vlad">
          <b-dropdown-item><router-link to="/">Home</router-link></b-dropdown-item>
          <b-dropdown-item><router-link to="/blog">Blog</router-link></b-dropdown-item>
          <b-dropdown-item><router-link to="/featured">Featured</router-link></b-dropdown-item>
          <b-dropdown-item><router-link to="/about">About</router-link></b-dropdown-item>
          <b-dropdown-item><router-link to="/privacy">Privacy</router-link></b-dropdown-item>
          <b-dropdown-item><router-link to="/contact">Contact</router-link></b-dropdown-item>
          </b-dropdown>
      </div>
   <router-view/>
   <br>
   <br>
   <Footsum msg="Codex Black Studio © 2020 All Rights Reserved" class="toenail"/>
</div>
</template>

<script>
import Footsum from '@/components/Footsum.vue'

export default {
  name: 'App',
  components: {
    Footsum
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  a {
    text-align: center;
    font-weight: bold;
    color: #dcdcdd;

    &.router-link-exact-active {
      
      color: #1670a0;
    }
    
  }
  ul {  
    border-radius: 6px;
    background-color: #484e4a;
    box-shadow: inset 0 0 10px #dcdcdd;
  }
  a:hover {
    color: #1670a0;
  }
  li:hover {
    background-color: #1670a0;
  }
  
   
}

.vlad {
  padding: 2em;
  padding-left: 25%;
}
 
.mudblood {
padding: 2em;
padding-right: 30%;
}

.toenail {
  padding: 2em;
  background-color: #484e4a;
}
</style>
