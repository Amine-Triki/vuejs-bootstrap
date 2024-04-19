<template>
    <div>
      <div v-for="project in projects" :key="project.id" class="mb-3">
        <div class="card" style="width: 18rem;">
          <img :src="project.image" class="card-img-top" :alt="project.title">
          <div class="card-body">
            <h5 class="card-title">{{ project.title }}</h5>
            <p class="card-text">{{ project.description }}</p>
            <a :href="project.link" target="_blank" class="btn btn-primary">Visit</a>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        projects: [
          {
            id: 1,
            title: "site 1",
            description: "Vue js + BOOTSTRAP",
            image: "/src/assets/6.webp",
            link: "https://amine-triki.github.io/vuejs-bootstrap/"
          },
          {
            id: 2,
            title: "site 2",
            description: "WORDPRESS",
            image: "/src/assets/5.webp",
            link: "https://aminetriki.com.tn/"
          },
          {
            id: 3,
            title: "site 3",
            description: "WORDPRESS",
            image: "/src/assets/4.webp",
            link: "https://mjses.com"
          },
          {
            id: 4,
            title: "site 4",
            description: "JavaScript + BOOTSTRAP",
            image: "/src/assets/3.webp",
            link: "https://amine-triki.github.io/portfolio/"
          },
          {
            id: 5,
            title: "site 5",
            description: "JavaScript + BOOTSTRAP",
            image: "/src/assets/2.webp",
            link: "https://amine-triki.github.io/"
          },
          {
            id: 6,
            title: "site 6",
            description: "SASS + JavaScript",
            image: "/src/assets/1.webp",
            link: "https://amine-triki.github.io/portfolio-website-responsive-with-sass-js/"
          },
        ]
      };
    }
  };
  </script>
  
  <style scoped>

  </style>
