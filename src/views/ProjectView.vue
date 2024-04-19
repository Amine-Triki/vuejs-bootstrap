<template>
    <main>
      <section class="text-center pt-5 pb-5">
        <div class="container">
          <div class="main-title mt-5 mb-5 position-relative">
            <h2>My Projects</h2>
            <p>What I build</p>
          </div>
          <div class="text-start">
              <AllProjects class="mt-5 mb-5 d-flex justify-content-between flex-wrap" />
          </div>
        </div>
      </section>
    </main>
  </template>
  
  <script>
  import AllProjects from '../components/AllProjects.vue';
  
  export default {
    components: {
      AllProjects
    }
  };
  </script>
  
  <style scoped>
 
  </style>  