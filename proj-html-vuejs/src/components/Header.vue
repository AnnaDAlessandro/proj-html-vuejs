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
    </header>
  
</template>

<style scoped>
header{
    background-image: url(../img/avadabarbers-homepage-hero-bg.jpg);
    height: 200px;
}
.fa-cart-shopping{
    color: white;
}
#navbar{
    padding-top: 30px;
    margin: 0 auto;
    width: 70%;
}


</style>