<template>

    <div class="head">
        <h4>SUIVI DE LA COMMANDE</h4>
    </div>   
    <div class="general-infos">
    <div class="informations">
        <div class="commande">
            <p>N° de commande : 405560003 </p>
            <p> Date de commande :1 mai 2019</p>
            <p>Date d’expédition : 3 mai 2019</p>
            <p>Suivi commande</p>
            <p>Informations sur les retours</p>
        </div>    
    </div>
    <div>
            <p>ARTICLES</p>
        <div class="articles" v-for="item in items" v-bind:key="item.id">
            <img :src="item.image" :alt="item.name">
            <ul>
                <li>{{item.name}}</li>
                <li>{{item.price}}</li>
                <li>taille{{item.taille}}</li>
                <li>Qté:{{item.qté}}</li>
            </ul>
            </div>
          </div>  
        </div>        
</template>

<script>
import datos from "../assets/json/articles.json"
export default {
    name: 'Datos',
    props: {
        msg: String
    },
    
    computed:{
        items(){
            return datos.map((item)=>{
                return item;
            })
        }
    }
    
}
</script>

<style lang="scss" scoped>
.head{
    padding-top: 40px;
    display: inline-block;
    position: relative;
}

h4::after,h4::before{
    content: '';
    position: absolute;
    width: 350px;
    height: 1px;
    background-color: black;
    top: 0.6em;
} 
h4::before{
    top:70px;
    left: -350px;
}
h4::after{
    top:70px;
    right: -350px;
}


.commande{
    left: -281px;
    flex-direction: column;
    padding-top: 100px;

}

.general-infos{
    display: flex;
    justify-content: space-around;
    padding-top: 40px;
    padding-bottom: 50px;
}

ul{
     list-style:none;
}
.articles{
    display: flex;
    flex-direction: column;
    width: 522px;
    height: 152px;
    box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);
    
}
img{
    width: 120px;
    height: 100px;
}

 
</style>