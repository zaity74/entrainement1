<template>
  <div class="equipe_page">
      <h1 class="titre">Equipe</h1>

        <p v-if="display ==true">Message affichagé si condition vraie</p>

      <div class="card_box" v-if="users.length != 0">
          <Card v-for="card in users" :key="card.id" :card_email="card.email" :card_name="card.name"/>
      </div>

      <div class="card_box" v-if="userFiltered.length != 0">
          <Card v-for="card in userFiltered" :key="card.id" :card_email="card.email" :card_name="card.name"/>
      </div>
    
    <button @click="display = !display">Cacher / afficher le texte</button>
    <div v-if="display">
        texte a afficher ou a cacher
    </div>

      <button @click="filterName">
          click me
      </button>

  </div>
</template>

<script>
import axios from "axios"
import Card from "../components/Card"
export default {
    
    data() {
        return {
            users : [],
            userFiltered : [],
            display : false
        }
    },
    mounted(){
        axios.get("https://jsonplaceholder.typicode.com/users").then(response =>(
            this.users = response.data
        ))
    },
    methods: {
        filterName() {
            this.userFiltered = this.users.filter((element)=>{
                return element.name === "Leanne Graham"
            })

            this.users = []
        }
    },
    components: {
        Card
    }        

}

</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.equipe_page{
  position: relative;
  overflow-x: hidden;
}
.equipe_page .titre{
    color: #F5F5F5; 
    text-transform: uppercase;
    font: normal normal bold 161px/193px Bison;
    z-index: 3;
    font-family: Arial, Helvetica, sans-serif;

}
.equipe_page .titre{
    font-size: 81px;

}
.equipe_page .card_box{
     margin: 30px auto;
    margin-bottom: 200px;
    display: grid;
    justify-content: center; 
    position: relative;
    padding: 1rem;
}


    @media all and (min-width: 1150px) and (max-width: 4200px){
    .equipe_page{
        width: 100%;
        min-height: 100vh;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 20px;
        position: relative;
        margin-top: 90px;
        background-color: rgb(82, 209, 231);
    }
    .equipe_page .titre{
        margin-top: 40px;
        font-size: 81px;
    }
    .equipe_page .card_box{
        height: auto;
        width: 100%;
        background-color: red;
        grid-template-columns: repeat(4, 270px);
        gap: 20px;
    }
}
    @media all and (max-width: 1150px){
        .equipe_page{
            max-width: 1150px;
            width: 100%;
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
        .equipe_page .btn{
            font-size: 38px;
            text-align: center;
        }
        .equipe_page .icone{
        position: absolute;
        top: 221px;
        z-index: 1;
        opacity: 0.6;
        filter: grayscale(20%);
    }
        .equipe_page .card_box{
        height: auto;
        width: 100%;
        background-color: red;
        grid-template-columns: repeat(1, 270px);
        gap: 20px;
    }
}

</style>