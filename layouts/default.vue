<template>
  <div class="home">
    <div class="navbar">
      <div class="lien_menu">
        <a href="/">Accueil</a>
        <a href="/equipe">Equipe</a>
        <a href="#">Contact</a>
      </div>
      <svg class="logo" xmlns="http://www.w3.org/2000/svg" width="144.664" height="145.344" viewBox="0 0 144.664 145.344"><defs><style>.a{fill:#0066b9;}</style></defs><path class="a" d="M51.5,88.962,15.641,116.906,0,109.116V36.29l15.579-7.851,35.61,28.005L107.571,0l37.093,14.775V130.321l-36.908,15.023Zm54.96,9.83V46.552L72.7,72.7l33.755,26.089Zm-89.58-9.4L34.62,73.259,16.877,55.578Z"/></svg>
    </div>
    <Nuxt />
    <div class="foot">
      <div class="link_footer">
        <a href="#">Vscode</a>
        <a href="#">Corporation</a>
        <a href="#">CGV</a>
        <a href="#">A propos</a>
        <a href="#">Equipe</a>
        <a href="#">Contact</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>
<style>
.home{
  background-color: #2C2C32;
  display: flex; 
  flex-direction: column;
  position: relative;
  margin: auto;
}
.home .navbar{
  z-index: 9999;
  position: fixed;
  top: 0;
}
.home .lien_menu a{
  height: 100%;
  display: flex; 
  align-items: center;
  justify-content: center;
  color: white;
}
.home .lien_menu a:hover{
background-color: #6C6C6C;
}


.home .foot .link_footer a{
  height: 100%;
  padding-left: 40px;
  padding-right: 40px;
  display: flex;
  align-items: center;
  font-weight: 600;
  color:#25252B;
  font-size: 21px;
}

@media all and (min-width: 1150px) and (max-width: 4200px){
  .home{
  max-width: 1520px;
  width: 100%;
  height: 100%;
}
  .home .navbar{
  max-width: 1520px;
  width: 100%;
  height: 90px;
  background-color: #25252B;
  display: flex;
  flex-direction: row-reverse; 
  justify-content: space-between;
  align-items: center;
}
  .home .lien_menu{
    height: 100%;
    display: flex;
    align-items: center;
    margin-right: 12%;
  }
  .home .lien_menu a{
  padding-left: 70px;
  padding-right: 70px;
  height: 100%;
  font-size: 25px;
}
  .home .logo{
    margin-left: 84px;
    margin-top: 48px;
    width: 145px;
    height: 145px;
    color: #0066B9;
  }
  .home .foot{
  max-width: 1520px;
  width: 100%;
  height: 79px;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items: center;
}
  .home .foot .link_footer{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
  }
}

@media all and (min-width: 592px) and (max-width: 1150px){
  .home{
  max-width: 1150px;
  width: 100%;
}
    .home .navbar{
      width: 100%;
      height: 90px;
      background-color: #0066B9;
      display: flex;
      flex-direction: row-reverse; 
      justify-content: center;
      align-items: center;
    }
    .home .lien_menu{
      width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .home .lien_menu a{
  height: 100%;
  font-size: 25px;
  padding-left: 8%;
  padding-right: 8%;
}
   .home .logo{
   display: none;
  }
    .home .foot{
  max-width: 1520px;
  width: 100%;
  height: auto;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items: center;
}
  .home .foot .link_footer{

  display: flex;
  flex-wrap: wrap;
  row-gap: 8px;
  }
}
@media all and (min-width: 448px) and (max-width: 592px){
  .home{
  max-width: 592px;
  width: 100%;
}
    .home .navbar{
      width: 100%;
      height: 90px;
      background-color: #0066B9;
      display: flex;
      flex-direction: row-reverse; 
      justify-content: center;
      align-items: center;
    }
    .home .lien_menu{
      width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
    .home .lien_menu a{
  padding-left: 8%;
  padding-right: 8%;
  height: 100%;
  font-size: 25px;
}
   .home .logo{
   display: none;
  }
    .home .foot{
  max-width: 1520px;
  width: 100%;
  height: auto;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items: center;
}
  .home .foot .link_footer{

  display: flex;
  flex-wrap: wrap;
  row-gap: 8px;
  }
}

@media all and (max-width: 448px){
  .home{
  max-width: 592px;
  width: 100%;
}
    .home .navbar{
      width: 100%;
      height: 90px;
      background-color: #0066B9;
      display: flex;
      flex-direction: row-reverse; 
      justify-content: center;
      align-items: center;
    }
    .home .lien_menu{
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
    .home .lien_menu a{
  padding-left: 4%;
  padding-right: 4%;
  height: 100%;
  font-size: 25px;
}
   .home .logo{
   display: none;
  }
    .home .foot{
  max-width: 1520px;
  width: 100%;
  height: auto;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items: center;
}
  .home .foot .link_footer{

  display: flex;
  flex-wrap: wrap;
  row-gap: 8px;
  }
}
</style>
