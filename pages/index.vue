
<template>
    <div>
      <div class="menu-geral">
        <Navigation>
          <ul class="menu">
            <li class="item">
              <NuxtLink class="menu-item" to="/">
                HOME
              </NuxtLink>
            </li>
            <li class="item">
              <NuxtLink class="menu-item" to="/sobreNos">
                SOBRE NÓS
              </NuxtLink>
            </li>
            <li class="item">
              <NuxtLink class="menu-item" to="/faleConnosco">
                FALE CONNOSCO
              </NuxtLink>
            </li>
            <li class="item">
              <NuxtLink class="menu-item" to="/contactos">
                CONTACTOS
              </NuxtLink>
            </li>
          </ul>
        </Navigation>
      </div>
      <main class="principal-area">
        <img class="principal-image" src="~/assets/banner.jpg" />
        <h1 class="text-up">
          WELCOME TO THE GAMMER WORLD

          <p>Hello Brabos aqui você vai encontrar tudo sobre o mundo gammer!</p>
        </h1>
      </main>
    </div>
</template>

<style>
  .item{
    display: inline-block;
    padding: 8px;
    color: grey;
    margin-right: 0px;
    float: right;
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
    padding: 16px;
  }
  .menu-item:hover
  {
    background-color: #BB07E6;
    border-radius: 8px;
    color: white;
    transition: 1s;
  }
  .principal-image{
    margin-left: auto;
    width: 100%;
    height: 5%;
  }
  .principal-area{
    margin-top: 3%;
    font-family: sans-serif;
  }
  .text-up{
    text-align: center;
    margin-top: -45%;
    color: white;
  }
  img {
    margin-bottom: 1rem;
  }
</style>

<script>
export default {}
</script>
