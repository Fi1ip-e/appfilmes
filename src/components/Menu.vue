<template>
  <div>
    <b-navbar toggleable="lg" variant="info" style="font-size: 18px">
      <b-navbar-brand href="#"
        ><img class="cart" src="/assets/iconCart.png" alt="carrinho"
      /></b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#"><strong>Home</strong></b-nav-item>
          <b-nav-item href="#"><strong>About</strong></b-nav-item>
          <b-nav-item href="#"><strong>Os mais vendidos</strong></b-nav-item>
          <b-nav-item href="#"><strong>Blu-ray</strong></b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <div class="pesquisa">
      <b-form-input size="sm" placeholder="Search"></b-form-input>
      <b-button size="sm" class="Bpesquisa" type="submit">Search</b-button>
    </div>
  </div>
</template>
<style scoped>
nav {
  background-color: #6a5acd !important;
  /* background-image: linear-gradient(#f1ac92, #0c0c0a) !important; */
}
h1,
h4 {
  text-align: center;
  color: aliceblue;
  text-shadow: #424040 0.1rem 0.2rem;
  margin-right: 3rem;
}
a {
  text-decoration: none;
  color: rgb(226, 222, 222);
}
.cart {
  width: 48px;
  height: 50px;
}
.pesquisa {
  width: 65%;
  margin: 1rem;
  border-radius: 0.5rem;
  border-top-style: solid;

  border-style: solid;
  border-width: medium;
  border-color: #6a5acd;
}
@media (min-width: 900px) {
  .pesquisa {
    width: 30%;
    margin: 1rem;
  }
}
</style>