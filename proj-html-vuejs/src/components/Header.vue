<script >
import HamburgerMenu from './HamburgerMenu.vue';

export default{
    name: 'Header',
    components: {
    HamburgerMenu,
  },
   
    
}

</script>

<template>
    <header>
        <div class="d-flex align-items-center justify-content-between" id="navbar">
            <figure>
                <img src="../img/avadabarbers-logo-x1.png" alt="">
            </figure>
             <div class="d-flex align-items-center gap-2 ">
                <i class="fas fa-cart-shopping"></i>
                <div>
                <HamburgerMenu />
             </div>
             



             </div>
        </div>
        <div class="d-flex flex-column justify-content-end gap-4">
            <div id="icone" class="d-flex flex-column gap-4">
               <div class="d-flex flex-column align-items-center gap-2" id="folder">
                    <i class="fas fa-folder-minus"></i>
                    <span>Demos</span>
                </div>
                <div class="d-flex flex-column align-items-center">
                    <div class="d-flex p-0 m-0">
                    <i class="fas fa-dollar-sign"></i>
                    <h5 class="nuemro">39</h5>   
                    </div>
                    <span>On Sale</span>
                    
                </div> 
            </div>
                
             </div>
             <div class="d-flex" id="foto">
                <div class="d-flex flex-column" id="testo-1">
                <h1>
                    Barber Shop
                </h1>
                <hr>
                <span>The Pinnacle of Male Grooming</span>
               <div>
                <button class="btn-learn-more">
                    Learn More
                </button>
               </div>

                </div>
                <figure class="immagine-1">
                    <img src="../img/avadabarbers_hero_focalmirror-600x825.png" alt="">
                </figure>
                
             </div>
    </header>
  
</template>

<style scoped>
header{
    background-image: url(../img/avadabarbers-homepage-hero-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;

}
.fa-cart-shopping{
    color: white;
}
#navbar{
    padding-top: 30px;
    margin: 0 auto;
    width: 70%;
}
#icone{
    align-self: flex-end;
}
#icone span{
    font-size: 10px;
}
#icone div{
    background-color: #B0B0B0;
    padding: 5px;
    margin-right: 10px;
    border-radius: 20%;

}
#icone h5{
    font-size: 15px;
    color:#65bc7b;
    font-weight: bold;
}
.fa-dollar-sign{
    font-size: 10px;
    color:#65bc7b;
    font-weight: bold;
}
#folder{
   height: 51px;
   width: 51px;
}
#foto{
    margin: 0 auto;
    width: 70%;
    
}
.immagine-1{
    margin-left: 80px;
}
#testo-1{
    margin-left: 50px;
    margin-top: 250px;
}
hr{
    color:#BE9359;
    width: 50%;
    border: 2px solid #BE9359;
    opacity: unset !important;
    
}
h1{
    color: white;
    font-size: 80px;
    font-weight: bold;
}
#foto span{
    color:white;
    padding-block: 20px;
    opacity: 0.25;
    font-size: 20px;
}
.btn-learn-more{
            margin-top: 10px;
            display: inline-block;
            padding: 10px 30px;
            text-align: center;
            text-decoration: none;
            color: #BE9359;
            border: 2px solid #BE9359;
            transition: opacity 0.3s ease;
            background: none;
            font-size: 15px;
            text-transform: uppercase;
        }

.btn-learn-more:hover {
            opacity: 0.7;
            font-size:18px;
}

</style>