<template>
    <div>
  <b-jumbotron class="Jumb">
      <h1><img class="cart" src="/assets/folder_movie.png" alt="log"
      /><strong>Store's de Filmes</strong></h1>
    <p>Sua Loja de filmes na palma da mão.</p>
    <p>Classicos, Comedia, Ação, Aventura, Lançamentos</p>
  </b-jumbotron>
</div>
</template>

<style scoped>
.Jumb {
    background-image: url("/assets/Cinema-vazio.jpg");
    background-position: 30% 30%;
    background-size: cover;
    color: #d3cfcf;
    /* background-image: linear-gradient(#4A708B, #C6E2FF); */
    align-items: center;
    text-align: center;
    padding-bottom: 1rem;
}
p {
    font-size: 20px;
    text-shadow: #141414 0.1rem 0.1rem;
}
h1 {
    
  text-align: center;
  font-size: 40px;
  text-shadow: #2b2a2a 0.1rem 0.1rem;
}

@media (min-width: 900px) {
    .Jumb {
    
    background-position: 30% 20%;
    padding-top: 2rem;
    padding-bottom: 2rem;
    font-size: 50px;
}
}
</style>