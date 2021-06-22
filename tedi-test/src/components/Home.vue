<template>
    <NavBar/>
     <div class="head">
       <div class="line">&nbsp;</div>
            <div class="leyende">SUIVI DE LA COMMANDE</div>
            <div class="line">&nbsp;</div>
    </div>
    <div class="general-infos">
      <CommandeInfo/>
      <ArticleList/>
    </div>   
    <Client/>
    <Informations/>
    <Footer/>
</template>

<script>
import NavBar from './NavBar.vue'
import CommandeInfo from './suivi/CommandeInfo.vue'
import ArticleList from './suivi/ArticleList.vue'
import Client from './Client.vue'
import Informations from './Informations.vue'
import Footer from './Footer.vue'

export default {
  name: 'navbar',
 components: {
    NavBar,
    CommandeInfo,
    ArticleList,
    Informations,
    Client,
    Footer
  }
}
</script>


<style scoped lang="scss">

.head{
    padding-top: 40px;
    display: inline-block;
    position: relative;
}



.general-infos{
    display: flex;
    justify-content: space-around;
    padding-top: 40px;
    padding-bottom: 50px;
    margin: auto;
    width: 980px;
}


h3 {
  margin: 40px 0 0;
}
ul {
  list-style:none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
