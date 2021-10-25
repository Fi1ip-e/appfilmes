<template>
  <div class="container">
    <div class="slide">
      <h2 class="legenda"><strong>Destaques</strong></h2>
      <b-carousel
        class="slide2"
        id="carousel-no-animation"
        style="text-shadow: 0px 0px 2px #000"
        no-animation
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          
          img-src="/assets/BlueValentine.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/Captainamerica.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/FactoryGirl.png"
        ></b-carousel-slide>
      </b-carousel>
    </div>

    <div class="slide">
      <h2 class="legenda"><strong>Laçamentos</strong></h2>
      <b-carousel
        class="slide2"
        id="carousel-no-animation"
        style="text-shadow: 0px 0px 2px #000"
        no-animation
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          
          img-src="/assets/avatar.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/jennifersbody.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/badteacher.png"
        ></b-carousel-slide>
        
      </b-carousel>
    </div>

    <div class="slide">
      <h2 class="legenda"><strong>Queridinhos</strong></h2>
      <b-carousel
        class="slide2"
        id="carousel-no-animation"
        style="text-shadow: 0px 0px 2px #000"
        no-animation
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          
          img-src="/assets/300.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/EpicMovie.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/castlevania.png"
        ></b-carousel-slide>
        <b-carousel-slide
          
          img-src="/assets/aquamarine.png"
        ></b-carousel-slide>
      </b-carousel>
    </div>
  </div>
</template>

<style scoped>
.container {
  background-image: linear-gradient(#f1f50c, #e9f0f3);
}
.slide {
  width: 180px;
  height: 20%;
  display: inline-table;
  margin: 2rem 0 0.5rem -1.8rem;
  padding: 0;
  align-items: center;
  text-align: center;
}
.slide2 {
  width: 160px;
  height: 150px;
  margin: 0 -1rem 0 0;

  display: inline-table;
}
@media (min-width: 500px) {
  .slide {
    width: 180px;
    height: 20%;
    display: inline-table;
    margin: 2rem 0 0.5rem -1.5rem;
    padding: 0;
    align-items: center;
    text-align: center;
  }
  .slide2 {
    width: 160px;
    height: 150px;
    margin: 0 -1rem 0 0;

    display: inline-table;
  }
}
@media (min-width: 700px) {
  .legenda {
    font-size: 23px;
  }
  .slide {
    width: 170px;
    height: 20%;
    margin: 2rem 0 -1rem 0;
    padding: 0;

    display: inline-table;
  }
  .slide2 {
    width: 170px;
    margin-bottom: 0;

    display: inline-table;
  }
}
@media (min-width: 768px) {
  .slide {
    width: 170px;
    height: 20%;
    margin: 2rem 0 -1rem 1.7rem;
    padding: 0;

    display: inline-table;
  }
  .slide2 {
    width: 180px;
    margin-bottom: 0;

    display: inline-table;
  }
}
@media (min-width: 800px) {
  .slide {
    width: 170px;
    height: 20%;
    margin: 2rem 1.5rem -1rem 2rem;
    padding: 0;

    display: inline-table;
  }
  .slide2 {
    width: 190px;
    height: 150px;
    margin-bottom: 0;

    display: inline-table;
  }

  @media (min-width: 900px) {
    .slide {
      width: 180px;
      height: 20%;
      margin: 2rem 1.5rem -1rem 2rem;
      padding: 0;

      display: inline-table;
    }
    .slide2 {
      width: 260px;
      height: 150px;
      margin-bottom: 0;

      display: inline-table;
    }
  }
}
@media (min-width: 1000px) {
  .slide {
    width: 180px;
    height: 20%;
    margin: 2rem 1.5rem -1rem 1rem;
    padding: 0;

    display: inline-table;
  }
  .slide2 {
    width: 260px;
    height: 150px;
    margin-bottom: 0;

    display: inline-table;
  }
}
@media (min-width: 1200px) {
  .slide {
    width: 180px;
    height: 20%;
    margin: 1rem 1.5rem -1rem 4rem;
    padding: 0;

    display: inline-table;
  }
  .slide2 {
    width: 260px;
    height: 150px;
    margin-bottom: 0;

    display: inline-table;
  }
}
</style>