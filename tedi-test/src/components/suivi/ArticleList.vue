<template>   
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
</template>

<script>
import datos from "../../assets/json/articles.json"
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
ul{
     list-style:none;
}
.articles{
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 422px;
    height: 152px;
    box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);
    
}
img{
    width: 120px;
    height: 100px;
    padding-top: -50px;
}

 
</style>