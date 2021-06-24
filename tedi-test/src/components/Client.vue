<template>
    <div class="livraison">
			<div class="line">&nbsp;</div>
            <div class="leyende">
                INFORMATIONS SUR LA LIVRAISON
                <img src="/images/zigzag.svg" alt="/images/zigzag.svg">
            </div>
            <div class="line">&nbsp;</div>
    </div> 
    <div class="client" v-for="item in items" v-bind:key="item.id">
        <br>
        <div class="client-div">ADRESSE DE COLLECTE<br><br> {{item.collecte}}</div>
        <div class="client-div">VOS COORDONNÉES<br><br>{{item.client}}</div>
        <div class="client-div">LIVRAISON ESTIMÉE<br><br>{{item.estim}}</div>
        <div class="client-div">MODE DE LIVRAISON<br><br>livraison standard en point relais</div>
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
        padding-bottom: 20px;
    }
    .client{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-around;
        margin: auto;
        width: 980px;
        height: 152px;
        box-shadow: 0px 2px 4px 2px rgba(127, 124, 137, 0.227);
    }

    div .client-div{
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        max-width: auto;
        border-right: thin solid black ;
    }
    @media screen and (max-width: 600px){
        .client{
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 70%; 
            height: 400px;
        }
        .client .client-div{
            border-right: none;
            border-bottom:thin solid black;
            padding-bottom: 25px;
           }
    }
   
    
</style>