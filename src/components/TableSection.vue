<template >
  <div class="results__section">
    <div class="results__wrapper">
      <div class="results__section__header">
        <span id="result_last_update">Datos actualizados a las 11:03:04pm.</span>
      </div>
      <div class="results__section__table">
        <div class="table__header">
          <div class="header_data">
            Nombre
          </div>
          <div class="header_data">
            Compra
          </div>
          <div class="header_data">
            Venta
          </div>
          <div class="header_data">
            Spread
          </div>
          <div class="header_data">
            Pagina
          </div>
        </div>
        <div class="table__body">
          <div class="card">
            <div class="company__name">
              <img src="../assets/casas_cambio/inkamoney.png" alt="inkamoney">
            </div>
            <div class="buy-currency">
              <span>
                S/ 3.7180
              </span>
            </div>
            <div class="sell-currency">
              <span>
                S/ 3.7330
              </span>
            </div>
            <div class="spread">
              <span>
                S/ 0.0150
              </span>
            </div>
            <div class="link">
              <span>
                <a href="https://www.inkamoney.com/" target="_blank">Visitar</a>
              </span>
            </div>
          </div>
          
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style>
  .results__section{
    width: 100%;
    min-width: 1350px;
    
  }
  .results__wrapper{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .results__section__header{
    background-color: #00CB75;
    width: 70%;
    padding: 1rem 2rem; 
  }

  #result_last_update{
    color: #232323;
    font-weight: 500;
    font-size: 1rem;
    letter-spacing: 1px;
  }

  .results__section__table{
    width: 75%;
    justify-content: center;
  }

  .table__header{
    display:flex;
    width: 100%;
    justify-content: space-around;
    padding: 15px 0;
    margin-top: .5rem;
    border-top: 1px solid grey;
    border-bottom: 1px solid grey;
  }

  .table__header .header_data{
    margin-left: 30px;
    letter-spacing: 1px;
  }

  .table__body{
    display: flex;
    width: 100%;
    justify-content: center;
    margin-top: .9rem;
    flex-direction: column;
  }
  
  .card{
    box-shadow: rgba(0, 0, 0, 0.25) 0px 14px 28px, rgba(0, 0, 0, 0.22) 0px 10px 10px;
    border-radius: 10px;
    transition: 0.3s;
    display: flex;
    justify-content: space-around;
    padding: 0;
    margin: 5px 0;
    background-color: #fff;
    vertical-align: middle;
  }

  .card:hover{
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }

  .card .company__name {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 115px;
    margin-left: 15px;
    /* border: 1px solid black; */
  }

  .card .buy-currency{
    height: 100%;
    line-height: 100px;
    margin-right: 20px;
    /* border: 1px solid black; */
  }

  .card .buy-currency span{
    display: inline-block;
    vertical-align: middle;
    line-height: 20px;
    color: #00CB75;
  }

  .card .sell-currency{
    height: 100%;
    line-height: 100px;
    margin-right: 20px;
    /* border: 1px solid black; */
  }

  .card .sell-currency span{
    display: inline-block;
    vertical-align: middle;
    color: rgb(221, 3, 3);
    line-height: 20px;
  }
  
  .card .spread{
    height: 100%;
    line-height: 100px;
    /* border: 1px solid black; */
  }

  .card .spread span{
    display: inline-block;
    vertical-align: middle;
    color: #232323;
    line-height: 20px;
  }

  .card .link{
    height: 100%;
    line-height: 100px;
  }

  .card .link span{
    display: inline-block;
    vertical-align: middle;
    line-height: 20px;
    
  }

  .link span a {
    background-color: #00CB75;
    text-decoration: none;
    color: #fff;
    border-radius: 15px;
    font-weight: 600;
    padding: 8px 14px;
  }

  .link span a:hover{
    background-color:#069c5e;

  }

  

</style>