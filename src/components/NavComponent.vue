<template lang="js">
  <header>
    <div class="logo">
      <img src="@/assets/cambio-de-dinero_64px.png" alt="cambio-dolares">
      <a href="#" class="header__logo">
      <span style="color:#A9DE32;">Cambia</span>  
      Tu
      <span style="color:#00CB75">Dolar</span>
      </a>
    </div>
    <nav :class="nav" id="nav-menu">
      <ion-icon @click="clickMenu(true)" name="close-outline" id="close-menu" class="header__close"></ion-icon>
      <ul class="nav__list">
        <li class="nav__item"><a href="#" class="nav__link">Inicio</a></li>
        <li class="nav__item"><a href="#" class="nav__link">Acerca de</a></li>
        <li class="nav__item"><a href="#" class="nav__link">Contacto</a></li>
        <li class="nav__item"><a href="#" class="nav__link">NewsLetter</a></li>
      </ul>
    </nav>

    <ion-icon @click="clickMenu(false)" name="menu-outline" class="header__toggle" id="toggle-menu"></ion-icon>
  </header>
</template>
<script>

export default {
  data() {
    return {
      nav: ['nav']
    }
  },
  methods: {
    clickMenu(value){
      if(value) this.nav.pop()
      else this.nav.push('show')
    }
  },
}
</script>
<style scoped>
  a{
    text-decoration: none;
  }

  ul{
    list-style: none;
  }

  header{
    display: flex;
    background-color: #222831;
    justify-content: space-around;
    padding: .8rem 0;
    align-items: center;
  }

  .logo{
    display: flex;
    align-items: center;
  }

  .logo img {
    width: 50px;
    border-radius: 50%;
    margin-right: 10px;
  }

  .header__logo {
    color: #eee;
    font-weight: 600;
  }

  .nav__list{
    display: flex;
    align-items: center;
  }

  .nav__item{
    margin: 0 8px;
  }


  .nav__link {
    padding: 10px;
    color: #eee;
    font-size: 0.9rem;
    font-weight: 500;
    border-radius: 5px;
  }

  .nav__link:hover{
    background-color: #00CB75;
    color: #fff;
  }

  .header__toggle,
  .header__close{
    display:none;
  }

  @media screen and (max-width: 768px){
    header{
      height: 48px;
      justify-content: space-between;
      padding: 0 28px;
    }

    .logo a {
      font-size: 0.9rem;
    }

    .logo img {
      width: 30px;
    }

    .header__toggle {
      display: inline;
      color: #eee;
      font-size: 24px;
    }

    .header__close{
      position: absolute;
      right: 24px;
      display: block;
      font-size: 24px;
      border-radius: 50%;
    }

    .header__close:hover{
      background-color: #00CB75;
      color: #eee;      
    }

    .nav{
      position: fixed;
      top:0 ;
      right: -100%;
      background-color: #222831;
      color: #eee;
      width: 60%;
      height: 100vh;
      padding: 24px 0;
      z-index: 100;
      transition: 0.5s;
      border-radius: 0 0 0 50%;
    }

    .nav__list {
      display: flex;
      flex-direction: column;
    }

    .nav__item {
      margin: 2rem 0;
    }

    .show{
      right: 0;
    }

  }




</style>