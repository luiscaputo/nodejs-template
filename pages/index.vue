
<template>
    <div>
      <div class="menu-geral">
        <Navigation>
        <ul class="menu">
          <li class="item"><NuxtLink class="menu-item" to="/">HOME</NuxtLink></li>
          <li class="item"><NuxtLink class="menu-item" to="/sobreNos">SOBRE NÓS</NuxtLink></li>
          <li class="item"><NuxtLink class="menu-item" to="/faleConnosco">FALE CONNOSCO</NuxtLink></li>
          <li class="item"><NuxtLink class="menu-item" to="/contactos">CONTACTOS</NuxtLink></li>
        </ul>
      </Navigation>
      </div>
      <h1>Hello Nuxters! 👋</h1>
      <p>
        This page is rendered on the <strong>{{ rendering }}</strong>
      </p>
      <p v-if="rendering === 'server'">
        First load or hard refresh is done on server side.
      </p>
      <p v-if="rendering === 'client'">Navigation is done on client side.</p>
      <ul>
        <li>Refresh the page for server side rendering.</li>
        <li>Click the links to see client side rendering.</li>
      </ul>

      <NuxtLink to="/my-profile">About Page</NuxtLink>
  </div>
</template>

<style>
  .item{
    display: inline-block;
    padding: 8px;
    color: grey;
    margin-right: 20px;
  }
  .menu-geral{
    width: 960px;
    margin-left: auto;
    margin-right: auto;
    padding: 4px;
    font-family: sans-serif;
  }
  .menu-item{
    text-decoration: none;
    color: black;
    padding: 8px;
  }
  .menu{
    padding: 8;
  }
</style>

<script>
export default {}
</script>
