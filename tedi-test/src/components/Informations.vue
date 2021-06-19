<template>
    <div class="paiement-header">
			<h4>INFORMATIONS DE PAIEMENT</h4>
	</div> 
    <div>
        VISA
    </div>
	
	<div class="paiement-info">
		<h4>TOTAL COMMANDE</h4>
	</div>  
    <div id="Sous-totale_Livraiso">
		<span>Sous-totale<br/><br/>Livraison<br/></span><br><span style="font-family:GillSansStd;">TOTAL : </span>
	</div>
    <div id="Sous-totale_Livraiso">
		<span>Sous-totale<br/><br/>Livraison<br/></span><br><span style="font-family:GillSansStd;">TOTAL : </span>
	</div>
	<div id="ID1130_GRATUITE_1130">
		<span>1130<br/><br/>GRATUITE<br/></span><br><span style="font-family:GillSansStd;">1130</span>
	</div>
</template>

<script>
export default {

}
</script>

<style>
.paiement-header{
        display: inline-block;
        position: relative;
	}
.paiement-info{
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