<template>
  <footer class="footer pt-2 pb-2 bg-success">
    <p id="Rights" class="container text-center">
      {{ year }} &copy; Amine Triki || All Rights Reserved
    </p>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter',
  data() {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>