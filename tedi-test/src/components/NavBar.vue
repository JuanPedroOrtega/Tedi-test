<template>
    <div class="box">
        <ul id="Menu" class="Menu shadow" >
            <li class="logo">
                <img src="@/assets/tediber.svg" alt="tediber">
            </li>
            <li>
                <span>NOS PRODUITS</span>
                <ul class="dropdown">
                    <li></li>
                    <li></li>
                </ul>
                <button> </button>
            </li>
            <li>
                <span>LE CONCEPT</span>
            </li>
            <li>
                <span>AVIS</span>
            </li>
            <li class="ours">
                <img src="@/assets/tedi.svg" alt="logo">
            </li>
            <li>
                <span>CONTACTEZ-NOUS</span>
            </li>
            <li>
                <span>MAG</span>
            </li>
            <li>
                <span>MON COMPTE</span>
            </li>
            <li>
                <span>PUB TV</span>
            </li>
            <li class="bolsa">
                <img src="@/assets/bag.svg" alt="bag">
            </li>    
        </ul>
    </div>
    
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .mediaViewInfo {
		--web-view-name: Web 1920 – 1;
		--web-view-id: Web_1920__1;
		--web-scale-on-resize: true;
		--web-enable-deep-linking: true;
	}
	:root {
		--web-view-ids: Web_1920__1;
	}
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		border: none;
    }
    .box{
        filter: drop-shadow(0px 2px 4px rgba(127, 124, 137, 0.227));
		position: absolute;
		overflow: visible;
		width: 1212px;
		height: 92px;
		left: 0px;
        top: 0px;
        width: 100%;
    }
	#Menu {
        list-style:none;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        width: 100%;
        box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);
    }
    
    .dropdown{
        border: 0.1em solid black;
        width: 10em;
        margin-bottom: 1em;
    }
    
    
</style>