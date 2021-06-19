<template>
    <div class="livraison">
			<h4>INFORMATIONS SUR LA LIVRAISON</h4>
    </div> 
    <div class="client" v-for="item in items" v-bind:key="item.id">
        <span>ADRESSE DE COLLETCTE {{item.collecte}}</span>
        <span>VOS COORDONNÉES{{item.client}}</span>
        <span>LIVRAISON ESTIMÉE{{item.estim}}</span>
        <span>MODE DE LIVRAISON</span>
    </div>
</template>

<script>
import datos from "../assets/json/infoclient.json"
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

<style>
    .livraison{
        display: inline-block;
        position: relative;
    }
    h4::after,h4::before{
    content: '';
    position: absolute;
    width: 300px;
    height: 1px;
    background-color: black;
    top: 0.6em;
    } 
    h4::before{
    top:30px;
    left: -330px;
    }
    h4::after{
    top:30px;
    right: -330px;
    }
    .client{
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 822px;
    height: 152px;
    box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);
    }

    
</style>