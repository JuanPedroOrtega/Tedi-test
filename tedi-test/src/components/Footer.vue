<template>
	<div class="footer-header">
		<div class="line">&nbsp;</div>
		<div class="leyende">
			BESOIN D'AIDE ?
			<img src="/images/zigzag.svg" alt="/images/zigzag.svg">
		</div>
		<div class="line">&nbsp;</div>
	</div>
	<nav class="footer-nav">
		<div class="menu-footer">
			<a href="#">FOIRE AUX QUESTIONS TEDIBER</a>
		</div>
		<div class="menu-footer">
			<a href="#">LA GARANTIE TEDIBER</a>
		</div>
		<div class="menu-footer">
			<a href="#">REPRISE DE L’ANCIENNE LITERIE</a>
		</div>
		<div class="menu-footer">
			<a href="#">COMMENT FAIRE UN RETOUR ?</a>
		</div>
	</nav>
  
</template>

<script>
export default {

}
</script>

<style>
	.footer-header{
	display: inline-block;
	position: relative;	
	padding-bottom: 20px;
	}
	nav .menu-footer{
        color: black;
        position: relative;
        text-align: center;
	}
	nav .menu-footer a{
        color: inherit;
        text-decoration: none;
	}
	.footer-nav a {
    border-bottom: 1px solid #333;
    color: rgba(255,255,255,.5);
	display: block;
	width: 980px;
    font-size: 13px;
    margin-bottom: 5px;
	padding-bottom: 10px;
	margin: auto;
}
   
</style>