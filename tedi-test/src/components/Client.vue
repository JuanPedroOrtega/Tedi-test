<template>
    <div class="livraison">
			<h4>INFORMATIONS SUR LA LIVRAISON</h4>
    </div> 
    <div id="Adresse_de_colletcte">
		<span style="text-transform:uppercase;">Adresse de colletcte</span><br><span></span><br><span style="font-family:GillSansStd-Light;">POINT RELAIS57 rue Jean Pierre Timbaud<br/>PARIS<br/>75011<br/>France</span>
	</div>
	<div id="vos_coordonnes_Shan">
		<span style="text-transform:uppercase;">vos coordonnées</span><br><span></span><br><span style="font-family:GillSansStd-Light;">Shannon Honniball <br/>0664262272</span>
	</div>
	<div id="livraison_estime_je">
		<span style="text-transform:uppercase;">livraison estimée</span><br><span></span><br><span style="font-family:GillSansStd-Light;">jeudi 9 mai 2019</span>
	</div>
	<div id="mode_de_livraison_li">
		<span style="text-transform:uppercase;">mode de livraison</span><br><span></span><br><span style="font-family:GillSansStd-Light;">livraison standard en point relais</span>
	</div>
</template>

<script>
export default {

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
    width: 350px;
    height: 1px;
    background-color: black;
    top: 0.6em;
} 
h4::before{
    top:30px;
    left: -350px;
}
h4::after{
    top:30px;
    right: -350px;
    }
</style>