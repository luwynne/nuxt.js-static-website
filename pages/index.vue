<template>
  <div class="container">
    
    <main>
      <h1>This is a website made using Nuxt.js</h1>
      <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
    </main>
  </div>
</template>

<script>


export default {
  components: {
    
  },
  // this displays the title of the page on the browser tab
  head(){
      return {
        title: 'Nuxt Website | Home'
      }
  }
}
</script>

<style>
/*.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}*/



</style>
