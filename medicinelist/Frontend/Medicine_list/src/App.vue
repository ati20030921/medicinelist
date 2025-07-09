<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <HelloWorld />
      <nav class="navbar navbar-expand-sm bg-dark navbar-light">
        <div class="container-fluid">
          <ul class="navbar-nav">
            <li class="nav-item">
              <RouterLink to="/" class="nav-link text-light">Home</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink to="/application" class="nav-link text-light" >Appliaction</RouterLink>
            </li>
          </ul>
          <div>
          <button src="../src/views/Registration.vue" class="btn btn-primary" type="button">Login / Registration</button>          
            </div>
        </div>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>

.navbar{
  height: 100px;
}

.nav-link{
  font-size: 25px;
}

.btn{
  background-color: black;
  color: white;
  height: 60px;
  font-size: 25px;
}
</style>


