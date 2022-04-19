<template>
  <div class="mobile_container">
    <div class="data_info_banner">
      <p>
        Datos actualizados a las 17:24:00pm.
      </p>
      <span>
        (El precio web se actualizara en 00:30)
      </span>
    </div>
    <div class="header_table_companies">
      <a href="#" class="buys active">Compra</a>
      <a href="#" class="sells">Venta</a>
    </div>
    <div class="currency_company">
      <img src="../assets/casas_cambio/inkamoney.png" alt="inkamoney">
      <div class="currency_data">
        <span class="buy_currency">
          S/ 3.7180
        </span>
        <span class="sell_currency">
          S/ 3.7330
        </span>
        <a target="_blank" class="visit_btn" href="https://www.inkamoney.com/">
          Ir a
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      
    }
  },
}
</script>
<style scoped>

  .mobile_container{
    margin: 0 auto;
    padding-top: 2rem;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 90%;
  }
  

  .data_info_banner span{
    margin-top: 0.2rem;
    padding: 0;
  }

  .header_table_companies{
    background-color: #222831;
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 5rem;
    margin: 5px;
    margin-top: 1.2rem;
    border-radius: 10px;
    width: 95%;
  }

  .header_table_companies a{
    color: #fff;
    text-decoration: none;
    font-weight: 600;
    font-size: 16px;
    transition: all 0.3s ease;
    padding: 5px;
    
  }

  .header_table_companies  a.active {
    color: #00CB75;
    border-bottom: 1px solid;
  }

  .currency_company{
    display: flex;
    align-items: center;
    justify-content: space-around;
    margin: 1rem;
    gap: 2rem;
    width: 100%;
    max-width: 90%;
    background-color: #fff;
    padding: 1rem;
    border-radius: 15px;
    box-shadow: rgba(0, 0, 0, 0.25) 0px 14px 28px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
  }

  .currency_data{
    display: flex;
    flex-direction: column;
    gap: 1rem
  }

  .currency_data span{
    font-weight: 600;
  }

  .currency_data span.buy_currency{
    color: #00CB75;
  }
  .currency_data span.sell_currency{
    color: rgb(221, 3, 3);
  }

  .currency_data .visit_btn{
    color:#fff;
    background-color: #232323;
    padding: 5px 8px;
    text-align: center;
    box-shadow:  rgba(0, 0, 0, 0.25) 0px 7px 14px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
    text-decoration: none;
    border-radius: 10px;
  }

  


</style>