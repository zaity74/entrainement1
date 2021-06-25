<template>
  <div class="home_box">
      <h1 class="titre">Vscode team</h1>
      <p>Devenez un dev ninja</p>
      <button class="btn">Rejoignez l'équipe</button>
      <img src="@/assets/image/screenshot.png"  width="200" alt="" class="image_music" >
      <svg class="icone" xmlns="http://www.w3.org/2000/svg" width="804.812" height="808.595" viewBox="0 0 804.812 808.595"><defs><style></style></defs><path class="a" d="M286.5,494.925,87.016,650.384,0,607.048V201.891l86.672-43.68,198.108,155.8L598.45,0,804.812,82.2V725.019L599.482,808.6Zm305.76,54.686V258.984L404.47,404.47l187.79,145.141ZM93.895,497.333l98.71-89.767L93.895,309.2Z"/></svg>

  </div>
</template>

<script>
export default {

}
</script>

<style >
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.home_box{
  position: relative;
  overflow-x: hidden;
}
.home_box .titre{
    color: #F5F5F5; 
    text-transform: uppercase;
    font: normal normal bold 161px/193px Bison;
    z-index: 3;
    font-family: Arial, Helvetica, sans-serif;
    text-align: left;

}
.home_box p{
  color: #F5F5F5; 
  text-transform: uppercase;
  z-index: 3;

}
.home_box .btn{
  background-color: #0066B9; 
  font: normal normal 300 38px/46px Helvetica;
  width: 560px;
  outline: none;
  border: none;
  height: 86px;
  color: white;
  z-index: 3;

}
.home_box .btn:hover{
  border: 2px rgb(73, 73, 214) solid;

}
.home_box img{
  margin: auto;
  width: 1268px;
  height: 776px;
  margin-bottom: 20px;
  z-index: 3;

}


    @media all and (min-width: 1150px) and (max-width: 4200px){
    .home_box{
        width: 100%;
        min-height: 100vh;
        height: 100%;
        display: flex;
        flex-direction: column;
        row-gap: 20px;
        position: relative;
        margin-top: 90px;
        background-color: red;
    }
    .home_box .titre{
        margin-top: 256px;
        margin-left: 281px;
        font-size: 81px;
    }
    .home_box p{
        font-size: 38px;
        padding-left: 281px;
    }
    .home_box .btn{
        font-size: 38px;
        margin-left: 281px;
        text-align: left;
        padding-left: 20px;
    }
    .home_box .icone{
        position: absolute;
        left: 60%;
        top: 221px;
        z-index: 1;
        opacity: 0.6;
        filter: grayscale(80%);
    }
}
    @media all and (min-width: 780px) and (max-width: 1150px){
        .home_box{
            width: 100vh;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            row-gap: 20px;
            position: relative;
            padding-top: 256px;
            margin-top: 90px;
            background-color: red;
        }
        .home_box .titre{
            font-size: 81px;
        }
        .home_box p{
            font-size: 38px;
        }
        .home_box .btn{
            font-size: 38px;
            text-align: center;
        }
        .home_box .icone{
        position: absolute;
        top: 221px;
        z-index: 1;
        opacity: 0.6;
        filter: grayscale(20%);
    }
}
    @media all and (max-width: 780px){
        .home_box{
            width: 100vh;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            row-gap: 20px;
            position: relative;
            padding-top: 256px;
            margin-top: 90px;
            background-color: red;
        }
        .home_box .titre{
            font-size: 80px;
        }
        .home_box p{
            font-size: 38px;
        }
        .home_box .btn{
            font-size: 38px;
            text-align: center;
        }
        .home_box .icone{
        position: absolute;
        top: 221px;
        z-index: 1;
        opacity: 0.6;
        filter: grayscale(20%);
    }
}
</style>
