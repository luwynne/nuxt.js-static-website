<template>
    <header>
        <h3 class="logo">Nuxt website</h3>
        <ul>
          <li>
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/about">About</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/contact">Contact</nuxt-link>
          </li>
           <li>
            <nuxt-link to="/donate">Donate</nuxt-link>
          </li>
        </ul>
    </header>
</template>

<style scoped>

  header{
    background: #77b6ea!important;
    color:#2b3d41;
    width: calc(100% - 14em);
    height: 8em;
    padding: 0 7em;
    display: flex;
     /* This makes the div behave as a row on display flex divs, such as display inline */
    flex-direction: row;
    justify-content: space-between;
     /* This is used for vertical align */
    align-items: center; 
   
  }

  h3.logo{
    font-size: 3em;
    font-weight: 300;
  }

  ul{
    padding: 0;
    margin: 0;
    list-style: none;
    display: flex;
    flex-direction: row;
  }

  li{
    padding: 1em .5em;
    font-size: 1.5em;
  }
  
  li a{
    padding: 1em .5em;
    color: inherit;
  }

</style>
    
