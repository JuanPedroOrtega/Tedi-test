<template>
    <div class="line-head">
		<div class="line">&nbsp;</div>
		<div class="leyende">INFORMATIONS DE PAIEMENT</div>
		<div class="line">&nbsp;</div>
			
	</div> 
    <div class="paiement-header">
		<img class="visa-logo" src="/images/visa.jpg" alt="/images/visa.jpg">
        VISA
    </div>
	
	<div class="paiement-info">
		<div class="line">&nbsp;</div>
		<div class="leyende">TOTAL COMMANDE</div>
		<div class="line">&nbsp;</div>
	</div>  
	<div class="resume">
		<div>
			<span>Sous-totale <span>1130</span></span>	
		</div>
		<div>
			<span>Livraison <span>GRATUITE</span></span>	
		</div>
		<div>
			<span>TOTAL <span>1130</span></span>
		</div>
	</div>
</template>

<script>
export default {

}
</script>

<style>
.line-head{
	display: inline-block;
	position: relative;	
	padding-bottom: 20px;
}
.paiement-header{
	display: inline-block;
	position: relative;
	display: flex;
	flex-direction: row;
	align-items: center;
	justify-content: initial;
	margin: auto;
	width: 980px;
	height: 35px;
	box-shadow: 0px 2px 4px 2px rgba(127, 124, 137, 0.227);
}
.paiement-info{
	display: inline-block;
	position: relative;
	padding-bottom: 20px;
}
.visa-logo{
	width: 30px;
}

.resume{
	display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    margin: auto;
    width: 980px;
    height: 152px;
    box-shadow: 0px 2px 4px 2px rgba(127, 124, 137, 0.227);
}

 @media screen and (max-width: 600px){
	.paiement-header{
		width: 70%;
	}
	.resume{
		width: 70%;
	}
 }


</style>