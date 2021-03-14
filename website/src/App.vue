<template>
  <div>

    <nav class="navbar navbar-expand-lg navbar-light bg-light" id="nav" style="position:sticky">
      <span class="navbar-brand mr-3" id="navbar-name"><router-link to="/">Gulliford Tutors</router-link></span>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <span class="nav-item nav-link active">
            <router-link to="/">Home</router-link>
          </span>
          <span class="nav-item nav-link">
            <router-link to="/about">About</router-link>
          </span>
          <span class="nav-item nav-link">
            <router-link to="/books">Books</router-link>
          </span>
          <span class="nav-item nav-link">
            <router-link to="/tests">Tests</router-link>
          </span>
        </div>
      </div>
    </nav>

    <div class="container-fluid mt-4">
      <router-view />
    </div>
  </div>
</template>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  #navbar-name a{
    margin-right: 30px !important;
    font-weight: bold !important;
    color: #232221 !important;
  }

  #nav {
    padding: 15px;
  }

    #nav a {
      font-weight: bolder;
      color: #232221;
      margin-right: 5px;
      text-decoration: none
    }

      #nav a.router-link-exact-active {
        color: #42b983;
      }
</style>
