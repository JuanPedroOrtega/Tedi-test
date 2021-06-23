<template>
    <nav class="navbar">
        <div class="hamburger">
            <div class="burguer">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </div>
            <div class="burguer-logo">
                <img class="logo" src="/images/tediber.svg" alt="tediber">
            </div>
            <div class="burguer-sac">
                <img class="bolsa" src="/images/bag.svg" alt="bag">
            </div>
        </div>
        <div class="nav-menu">    
            <div class="menu-item">
                <img class="logo" src="/images/tediber.svg" alt="tediber">
            </div>
            <div class="menu-item">
                <a class="dropdown" href="#">NOS PRODUITS</a>
                <div class="arrow"></div>
            </div>
            <div class="menu-item">
                <a href="#">LE CONCEPT</a>
            </div>
            <div class="menu-item">
                <a href="">AVIS</a>
            </div>
            <div class="menu-item">
                <img class="ours" src="/images/tedi.svg" alt="logo">
            </div>
            <div class="menu-item">
                <a href="#">CONTACTEZ-NOUS</a>
            </div>
            <div class="menu-item">
                <a href="#">MAG</a>
            </div>
            <div class="menu-item">
                <a href="#">MON COMPTE</a>
            </div>
            <div class="menu-item">
                <a href="#">PUB TV</a>
            </div>
            <div class="menu-item">
                <img class="bolsa" src="/images/bag.svg" alt="bag">
            </div>
        </div>
    </nav>
    
</template>

<script>
export default {
    name: 'navbar',
    data(){
        return{
        }
    }

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
    nav .nav-menu{
        list-style:none;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        width: 980px;
        box-shadow: 0px 2px 4px 2px rgba(127, 124, 137, 0.227);
        margin: auto;
    }

    nav .menu-item{
        color: black;
        position: relative;
        text-align: center;
    }
    /*.navbar{
        filter: drop-shadow(0px 2px 4px rgba(127, 124, 137, 0.227));
		position: absolute;
		overflow: visible;
		width: 1212px;
		
		left: 0px;
        top: 0px;
        width: 100%;
    }*/
    nav .menu-item a{
        color: inherit;
        text-decoration: none;
    }
    nav .menu-item:hover{
         color: goldenrod;
    }

    .ours:hover{
        transform: rotate(45deg);
    }
    
    .bolsa:hover{
        transform: rotate(25deg);
    }

    .hamburger {
        display: none;
    }

    .bar {
        display: block;
        width: 25px;
        height: 3px;
        margin: 5px auto;
        -webkit-transition: all 0.3s ease-in-out;
        transition: all 0.3s ease-in-out;
        background-color: #101010;
    }


     @media screen and (max-width: 600px) {
                .nav-menu .menu-item{
                position: fixed;
                left: -100%;
                top: 5rem;
                flex-direction: column;
                background-color: #fff;
                margin: auto;
                width: 100%;
                border-radius: 10px;
                text-align: center;
                transition: 0.3s;
                
            }
            .menu-item.active {
                left: 0;
                margin: 2.5rem 0;
            }
            .hamburger {
                display: flex;
                flex-direction: row;
                justify-content: space-between;
                width: 100%;
                box-shadow: 0px 2px 4px 2px rgba(127, 124, 137, 0.227);
            }
            

 
    }

</style>