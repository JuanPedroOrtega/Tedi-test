<template>
	<div class="footer-header">
		<h4>BESOIN D'AIDE ?</h4>
	</div>
  <div id="FOIRE_AUX_QUESTIONS">
		<span>FOIRE AUX QUESTIONS TEDIBER</span>
	</div>
	<div id="ARTICLES_4">
		<span>ARTICLES (4)</span>
	</div>
	<div id="Informations_sur_les">
		<span>Informations sur les retours</span>
	</div>
	<div id="LA_GARANTIE_TEDIBER">
		<span>LA GARANTIE TEDIBER</span>
	</div>
	<div id="reprise_de_lancienn">
		<span>reprise de l’ancienne literie</span>
	</div>
	<div id="comment_faire_un_ret">
		<span>comment faire un retour ?</span>
	</div>
</template>

<script>
export default {

}
</script>

<style>
	.footer-header{
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
    left: -380px;
    }
    h4::after{
    top:30px;
    right: -380px;
    
	}
</style>