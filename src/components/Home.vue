<template>
  <div class="container">
    <hr />
    <h2>
      <img src="/assets/iconPipoca.png" alt="iconPipoca" />
      <strong>Escolha Seus Filmes</strong>
    </h2>
    <hr />

    <div class="Filmes">
      <table
        v-for="item in myFilmes"
        :key="item"
        class="table table-borderless"
      >
        <tbody>
          <tr>
            <td>
              <img
                class="image-filme"
                v-bind:src="'/assets/' + item.image"
                v-bind:alt="item.image"
              />
            </td>
          </tr>
          <tr>
            <td class="name">
              {{ item.name }}
            </td>
          </tr>
          <tr>
            <td class="price">
              <strong>R$ {{ item.price }}</strong>
            </td>
          </tr>
          <div class="botoes">
            <a class="Bcomprar" href="#">
              <img
                class="iconComprar"
                src="/assets/icon_comprar.png"
                alt="iconComprar"
              />
              Comprar
            </a>
            <a placeholder="Add no carrinho" class="B-add" href="#">
              <img class="AddCart" src="/assets/cart.png" alt="carrinho" />
            </a>
          </div>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
import filmes from "../filmes.json";
export default {
  data: () => ({
    myFilmes: filmes,
  }),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
  text-align: center;
  color: aliceblue;
  background-image: linear-gradient(#4a708b, #c6e2ff);
  text-shadow: #424040 0.1rem 0.1rem;
}

hr {
  background-color: #14140e;
}
table {
  width: 20%;
  display: inline-table;
  margin: 0 0.8rem 1rem 0.5rem;

  padding-bottom: 0.8rem;
  color: black;
  font-size: 18px;

  align-items: center;
  text-align: center;

  border-top-style: solid;

  border-style: solid;
  border-width: medium;

  box-shadow: 0 1px 4px 3px rgb(73, 73, 73);
}
table:hover {
  box-shadow: 0 2px 10px 4px #b8d9fc;
}

.price {
  padding: 0.05rem 0 0.05rem 0;

  background-color: #858ce4;
  color: #fdf8f3;
  text-shadow: #070707 0.02rem 0.04rem;
}

.image-filme {
  width: 125px;
  height: 120px;
  margin: 0.08rem 0 -1rem 0;
}
.botoes {
  margin-bottom: 0.5rem;
  margin-top: 0.4rem;
  display: block;
}
.Bcomprar {
  display: block;
  margin: 0 0 0.8rem 0;
  text-decoration: none;
  background-color: #a9f719;
  color: rgb(19, 20, 20);
  border-radius: 0.5rem;
  font-size: 15px;

  border-top-style: solid;
  border-radius: 1rem;

  border-style: solid;
  border-width: medium;
  border-color: aliceblue;
}
.Bcomprar:hover {
  box-shadow: 0 2px 10px 2px #a9f719;
}
.AddCart {
  width: 25px;
  height: 25px;

  margin: 0;
  opacity: 0.9;
}
.B-add {
  background-color: #a9f719;

  margin: 0;
  padding: 0.4rem;

  border-radius: 0.5rem;
  border-top-style: solid;
  border-radius: 1rem;

  border-style: solid;
  border-width: medium;
  border-color: aliceblue;
}
.B-add:hover {
  box-shadow: 0 2px 10px 2px #a9f719;
}

.AddCart:hover {
  opacity: 0.5;
}
.iconComprar {
  padding: 0;
  width: 28px;
  height: 30px;
}
@media (min-width: 400px) {
  table {
    width: 20%;
    display: inline-table;
    margin: 0 0.8rem 1rem 1rem;

    padding: 0 0 0.8rem 0;
    align-items: center;
    text-align: center;
  }

  .price {
    padding: 0.05rem 0 0.05rem 0;
  }

  .image-filme {
    width: 140px;
    height: 130px;
    margin: 0.08rem 0 -1rem 0;
  }
  .botoes {
    margin-bottom: 0.5rem;
    margin-top: 0.4rem;
    display: block;
  }
  .Bcomprar {
    display: block;
    margin: 0 0 0.8rem 0;
  }
  .AddCart {
    width: 25px;
    height: 25px;

    margin: 0;
    opacity: 0.9;
  }
  .B-add {
    margin: 0;
    padding: 0.4rem;
  }
  .iconComprar {
    padding: 0;
    width: 28px;
    height: 30px;
  }
}
@media (min-width: 450px) {
  table {
    width: 2%;
    display: inline-table;
    margin: 0 0.8rem 1rem 2rem;

    padding: 0 0 0.8rem 0;
    align-items: center;
    text-align: center;
  }

  .price {
    padding: 0.05rem 0 0.05rem 0;
  }

  .image-filme {
    width: 140px;
    height: 130px;
    margin: 0.08rem 0 -1rem 0;
  }
  .botoes {
    margin-bottom: 0.5rem;
    margin-top: 0.4rem;
    display: block;
  }
  .Bcomprar {
    display: block;
    margin: 0 0 0.8rem 0;
  }
  .AddCart {
    width: 25px;
    height: 25px;

    margin: 0;
    opacity: 0.9;
  }
  .B-add {
    margin: 0;
    padding: 0.4rem;
  }
  .iconComprar {
    padding: 0;
    width: 28px;
    height: 30px;
  }
}

@media (min-width: 500px) {
  table {
    width: 20%;
    display: inline-table;
    margin: 0 0.8rem 1rem 0.5rem;

    padding-bottom: 0.8rem;
    align-items: center;
    text-align: center;
  }

  .price {
    padding: 0.05rem 0 0.05rem 0;
  }

  .image-filme {
    width: 125px;
    height: 120px;
    margin: 0.08rem 0 -1rem 0;
  }
  .botoes {
    margin-bottom: 0.5rem;
    margin-top: 0.4rem;
    display: block;
  }
  .Bcomprar {
    display: block;
    margin: 0 0 0.8rem 0;
  }
  .AddCart {
    width: 25px;
    height: 25px;

    margin: 0;
    opacity: 0.9;
  }
  .B-add {
    margin: 0;
    padding: 0.4rem;
  }
  .iconComprar {
    padding: 0;
    width: 28px;
    height: 30px;
  }
}

@media (min-width: 700px) {
  table {
    width: 23%;
    display: inline-table;
    margin: 0 0.5rem 1rem 2.5rem;
    padding: 0;
  }

  .image-filme {
    width: 165px;
    height: 150px;
  }
  .botoes {
    margin-top: -0.5rem;
  }
  .Bcomprar {
    display: block;
    margin: 1rem 0 0.5rem 0.1rem;
  }
  .B-add {
    margin-left: 0.5rem;
  }
  .AddCart {
    width: 35px;
    height: 40px;
    padding: 0;
  }
}
@media (min-width: 770px) {
  table {
    width: 23%;
    display: inline-table;
    margin: 0 0.5rem 1.5rem 2rem;
  }

  .image-filme {
    width: 160px;
    height: 150px;
  }

  .Bcomprar {
    display: block;
    margin: 1rem 0 0.5rem 0.1rem;
  }
  .B-add {
    margin-left: 0.5rem;
  }
  .AddCart {
    width: 35px;
    height: 40px;
    padding: 0;
  }
}

@media (min-width: 900px) {
  table {
    width: 23%;
    display: inline-table;
    margin: 0 0.5rem 1rem 2rem;
  }

  .image-filme {
    width: 160px;
    height: 150px;
  }

  .Bcomprar {
    display: block;
    margin: 1rem 0 0.5rem 0.1rem;
  }
  .B-add {
    margin-left: 0.5rem;
  }
  .AddCart {
    width: 35px;
    height: 40px;
    padding: 0;
  }
}
@media (min-width: 992px) {
  .navCart {
    background: "../assets/iconCart.png" !important;
  }
  table {
    width: 20%;
    height: 440px;
    display: inline-table;
    margin: 0 0.9rem 1rem 0.9rem;

    padding-bottom: 2rem;
    color: black;
    font-size: 20px;
  }

  .image-filme {
    width: 180px;
    height: 180px;
    margin: 0.1rem 0 -4.5rem 0;

    padding: 0;
  }
  .name {
    display: block;
    margin-top: 0;
    padding: 0;
  }
  .price {
    display: block;
    padding: 0 !important;
  }
  .botoes {
    margin-top: -1.5rem;
    
    padding: 0;
  }
  .Bcomprar {
    display: block;
    margin: 1.5rem 1rem 0.5rem 1rem;
    padding: 0.3rem;
  }

  .B-add {
    padding: 0.5rem;
  }
  .AddCart {
    width: 28px;
    height: 30px;

    margin: 0;
    opacity: 0.9;
  }
  .price {
    padding: 0.5rem 0 1rem 0;
  }
  .conteudo {
    font-size: 16px;
    padding: 0;
  }
}
@media (min-width: 1100px) {
  .navCart {
    background: "../assets/iconCart.png" !important;
  }
  table {
    width: 22%;
    display: inline-table;
    margin: 0 0.5rem 1rem 1rem !important;

    padding: 0;
    color: black;
    font-size: 20px;
  }
  .image-filme {
    width: 220px;
    height: 200px;
    margin: 0.1rem -1rem -3.5rem -1rem;

    padding: 0;
  }
  .AddCart {
    margin-top: 0;
    padding: 0;
  }
}
</style>
