<template>
  <nav  class="navbar navbar-expand-lg sticky-top navbar-dark  bg-success">
        <div class="container">
          <a class="navbar-brand" href="#"><h1>Amine Triki</h1></a>
          <button class="navbar-toggler" 
          type="button" 
          data-bs-toggle="collapse" 
          data-bs-target="#main" 
          aria-controls="main" 
          aria-expanded="false" 
          aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="main">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link p-2 p-lg-3">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/skills" class="nav-link p-2 p-lg-3">Skills</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/project" class="nav-link p-2 p-lg-3">Projects</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/contact" class="nav-link p-2 p-lg-3">Contact Me</router-link>
          </li>
        </ul>
          
          </div>
          
        </div>
  </nav>

</template>

<script>
export default {
    name : 'AppHeader'
}
</script>