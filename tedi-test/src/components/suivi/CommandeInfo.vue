<template>
  <div class="commande" v-for="item in items" v-bind:key="item.id">
      <ul>
            <li>
                <div class="but">
                    <p> N° de commande : {{item.num}} </p>
                </div>
            </li>
            <li>
                <div class="but">
                    <p> Date de commande :{{item.date}}</p>
                </div>
            </li>
            <li style="border-bottom: 1px solid #333;">
                <div class="but">
                    <p>Date d’expédition : {{item.expedition}}</p>
                </div>
            </li>
            <li style="border-bottom: 1px solid #333;">
                <div class="but">
                    <p>Suivi commande</p>
                    <span @click='toggle = !toggle' class="flecha-abajo" >
                        <img src="/images/chevron.svg" style="width:20px;" class="arrow" >
                    </span>
                </div>
                <div v-show='toggle' >
                    <ul class="details" >
                        <li class="etape"> 
                            <div class="stat">
                                <img src="/images/pack.svg" alt="/images/pack.svg">
                                <input type="checkbox" v-model="isChecked">
                            </div>
                            
                        </li>
                        <li class="etape">
                            <div class="stat">
                                <img src="/images/truck.svg" alt="/images/truck.svg">
                                <input type="checkbox" :checked="isChecked">
                            </div>
                        </li>

                        <li class="etape">
                            <div class="stat">
                                <img src="/images/route.svg" alt="/images/route.svg">
                                <input type="checkbox">
                            </div>
                        </li>
                        <li class="etape">
                            <div class="stat">
                                <img src="/images/packhouse.svg" alt="/images/packhouse.svg">
                                <input type="checkbox">
                            </div>    
                        </li>
                    </ul>
                </div>
            </li>
            <li style="border-bottom: 1px solid #333;">
                <div class="but">
                    <p>Informations sur les retours</p> 
                    <img src="/images/chevron.svg" style="width:20px" class="arrow" >
                </div>
            </li> 
      </ul> 
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
    },

   handleChange:function(){

   },
    data () {
   return {
     toggle: true,
     isChecked: true,
     active: false
   }
 },

}
</script>

<style lang="scss" scope>

ul{
    list-style: none;
}
li .etape{
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 10%;
}
.but{
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
    justify-content: space-between;
     width: 380px;

}
.commande{
    left: -281px;
    flex-direction: column;
    padding-top: 100px;
}
/*ul .details{
    display: none;
}*/
.details{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    margin: auto;
    width: 100%;
    position: relative;
   
}
.details img{
    width: 70px;
}

.flecha-abajo {
  border-top-width: 1em;
}
.flecha-abajo:hover{
    cursor: pointer;
}
.arrow:hover {
-moz-transform: rotate(180deg);
-ms-transform: rotate(180deg);
-webkit-transform: rotate(180deg);
transform: rotate(180deg);
}
@media screen and (max-width: 600px){
.details{
    display: flex;
    flex-direction: column;
   }
.stat{
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
}
}


</style>