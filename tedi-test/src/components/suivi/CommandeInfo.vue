<template>
  <div class="commande" v-for="item in items" v-bind:key="item.id">
            <p>N° de commande : {{item.num}} </p>
            <p> Date de commande :{{item.date}}</p>
            <p>Date d’expédition : {{item.expedition}}</p>
            <p>Suivi commande</p>
            <p>Informations sur les retours</p> 
    </div>
</template>

<script>
import datos from "../../assets/json/commande.json"
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

<style lang="scss" scope>

.commande{
    left: -281px;
    flex-direction: column;
    padding-top: 100px;
}
</style>