<template>
  <div>
    <Header/>
    <nuxt />
  </div>
</template>

<script>

import Header from '~/layouts/partials/Header.vue'

  export default{
    components: {
        Header
    },
    //head(){
      //return {
        //link: [ // adding links to the entire project
          //{
            //'rel': 'stylesheet',
            //'href': 'https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&display=swap'
          //}
        //]
      //}
    //},
    mounted () {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
  }
  }

</script>

<style lang="scss">
html {
  font-family: 'Lato';
  font-size: 16px;
}

body{
  width: 100%;
  height: 100vh;
  margin: 0;
  padding: 0;
}

.container{
  width: 100%;
  height: auto;

  main{
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    align-items: center;

    h1{
      font-size: 3em;
    }

    p{
      text-indent: 3em;
      font-size: 1.25em;
      line-height: 1.5em;
      margin-top: 0;
      padding-left: 50px;
      padding-right: 50px;
    }

  }

}

.page-enter-active{
  animation: bounce-in .8s;
}

.page-leave-active{
  animation: bounce-out .5s;
}

@keyframes bounce-in{
  0%{
    transform: scale(0);
  }
  50%{
    transform: scale(1.1);
  }
  100%{
    transform: scale(1);
  }
}

@keyframes bounce-out{
  0%{
    transform: scale(1);
  }
  50%{
    transform: scale(1.1);
  }
  100%{
    transform: scale(0);
  }
}


</style>
