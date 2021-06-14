<template>

    <div class="head">
        <span>SUIVI DE LA COMMANDE</span>
    </div>    
    <div class="informations">
        <div class="commande">
           <div>
                <span>N° de commande :</span><span style="font-family:GillSansStd;"> 405560003<br/></span><br><span>Date de commande :</span><span style="font-family:GillSansStd;"> 1 mai 2019<br/></span><br><span>Date d’expédition :</span><span style="font-family:GillSansStd;"> 3 mai 2019</span>
            </div>
            <div>
                <span>Suivi commande</span>
            </div>
        </div>
        <div class="article">
            <div>
                <span style="box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);"><img src="@/assets/5.jpg">L’incroyable OREILLER Tediber, 85 €, TAILLE : 60 x 60 cm; QTÉ : 2</span>
            </div>
            <div>
                <span style="box-shadow: 0px 2px 4px rgba(127, 124, 137, 0.227);"><img src="@/assets/couette.jpg">L’incroyable COUETTE Tediber;210 €;TAILLE : 240 x 220 cm;QTÉ : 1</span>
            </div>
        </div>  
    </div>      
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.head{
    display: flex;
    padding-top: 100px;
    align-items: center;
    padding-left: 620px;
}

.informations{
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-top: 50px;
}

.commande{
    display: flex;
    justify-content: flex-start;
    flex-direction: column;

}

.article{
    display: flex;
    justify-content: flex-end;
    flex-direction: column;
    align-content: flex-end;
    box-sizing: border-box;
}
img{
    width: 100px;
}

 
</style>