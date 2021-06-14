<template>
    <NavBar/>
    <Commande/>
    <Client/>
    <Informations/>
    <Footer/>
</template>

<script>
import NavBar from './NavBar.vue'
import Commande from './Commande.vue'
import Client from './Client.vue'
import Informations from './Informations.vue'
import Footer from './Footer.vue'

export default {
  name: 'navbar',
 components: {
    NavBar,
    Commande,
    Informations,
    Client,
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
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
