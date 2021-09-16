
<template>
    <div>
      <Navigation>
        <ul class="menu">
          <li class="item"><NuxtLink to="/">Pagina Inicial</NuxtLink></li>
          <li class="item"><NuxtLink to="/sobreNos">Sobre Nós</NuxtLink></li>
          <li class="item"><NuxtLink to="/faleConnosco">Fale Connosco</NuxtLink></li>
          <li class="item"><NuxtLink to="/contactos">Contactos</NuxtLink></li>
        </ul>
      </Navigation>
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
    text-decoration: none;
    font-family: 16pt;
    padding: 8px;
    background-color: blue;
  }
</style>

<script>
export default {}
</script>
