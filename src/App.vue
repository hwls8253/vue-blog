<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link to="/" class="nav-link active">home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/list" class="nav-link">list</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <router-view :blog="blog"></router-view>

  <!-- <List :blog="blog" /> -->
</template>
 
<script>
import blogData from './assets/blog.js';

export default {
  name: 'App',
  data() {
    return {
      blog : blogData
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
}
</style>
