<template>
  <section class="hero__container">
    <div class="hero__wrapper">
      <div class="hero__wrapper__right">
        <article class="hero__description">
          <h1 class="hero__description__title animate__animated animate__fadeInUp">
            Encuentra el mejor precio del <br>
            dolar con
            <span>
              nosotros.
            </span>
          </h1>
          <p class="hero__description__text">
            Si quieres conocer el precio del dolar, CambiaTuDolar te da la solución.
          </p>
          <p class="hero__description__text">
             
             Compara diferentes casa de cambio y encuentra la mejor opción.
          </p>
        </article>
        <article class="hero__calculator">
          <div class="calculator-section">
            <div class="calculator-header">
              <a href="#" data-currency="USD" data-operation="compra" class="currency-btn active">USD $</a>
              <a href="#" data-currency="PEN" data-operation="venta" class="currency-btn">PEN S/</a>
            </div>
            <div class="input-group-calculator">
              <input type="number" placeholder="0.00" value="1000">
              <input type="number" placeholder="0.00" value="269.11">
            </div>
            <div class="calculator-footer">
              <p>Mejor T. venta:  3.7160</p>
            </div>
          </div>
        </article>
      </div>
      <div class="hero__wrapper__left">
        <TableSection />
      </div>
    </div>
  </section>
  <MobileHero />
</template>
<script>
import TableSection from "./TableSection.vue";
import MobileHero from "./MobileHero.vue";

export default {
    components: { TableSection, MobileHero }
}
</script>
<style scoped>

  .hero__container{
    margin: 0 auto;
    width: 1350px;
    padding-top: 30px;
    height: auto;
  }
  
  .hero__wrapper{
    display: flex;
    flex-direction: column;
    width: 100%;
    justify-content: space-around;
    align-items: center;
  }

  .hero__wrapper__right {
    display: flex;
    gap: 100px;
    width: 90%;
    justify-content: space-evenly;
    align-items: center;
  }

  .hero__description{
    display: flex;
    flex-direction: column;
  }
  
  .hero__description__title{
    font-family: 'Dosis', sans-serif;
    font-weight: 500;
    color: #232323;
    font-size: 35px; 
  }

  .hero__description__title span {
    color: #00CB75;
  }

  .hero__description__text{
   font-family: 'Dosis', sans-serif;
    letter-spacing: 1px;
    margin: 0;
    padding: 5px;
    font-weight: 500;
    font-size: 18px;
  }

  .hero__description__text:last-child{
    margin-bottom: 2rem;
  }

  .calculator-section{
    width: 100%;
  }

  .calculator-header{
    display: flex;
    gap: 5px;
    flex-direction: row;
    justify-content:center;
    align-items: center;
  }

  .calculator-header a {
    text-decoration: none;
    padding: 10px 30px;
    border: 1px solid rgba(148, 148, 148, 0.671);
    width: 100%;
    
    text-align: center;
    color: #232323;
    
    font-weight: 700;
    border-radius: 5px;
  }

  .calculator-header a:hover {
    background-color: #00CB75;
    border: 1px solid #00CB75;
    color: #eee;
    transition: all .5s ease;
  }

  .calculator-header .active {
    background-color: #00CB75;
    border: 1px solid #00CB75;
    color: #eee;
  }

  .input-group-calculator{
    display: flex;
    flex-direction: column;
    margin-top: .5rem;
    gap: 5px;
  }

  .input-group-calculator input {
    padding: 10px;
    padding-right: 20px;
  } 

  @media screen and (max-width: 768px){
    .hero__container{
      display: none;
    }
    
  }


</style>