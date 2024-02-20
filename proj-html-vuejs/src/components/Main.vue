<script >
import Services from './Services.vue';
import Products from './Products.vue'
export default{
    name: 'Main',
    components: {
    Services,
    Products
  },
    data() {
        return{
            
        }
    
    },
}
</script>

<template>
    <main>
        
          <div id="pro-barber" class="col-md-12 text-center p-5">
            <span>AWARD WINNING</span>
            <h2>Pro Barbers</h2>
            <button class="btn-new-barber">MEET YOUR NEW BARBER</button>
        </div> 

        <Services></Services>
        <Products></Products>
      
        
        
    </main>
  
</template>

<style scoped>
 #pro-barber{
    background-image: url(../img/avadabarbers-about-introbackground.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    z-index: 1;
}
#pro-barber span{
    color:#BE9359 ;
}
#pro-barber h2{
    color: white;
    font-size: 70px;
}


 .btn-new-barber{
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

.btn-new-barber:hover {
            opacity: 0.7;
            font-size:18px;
}
.container {
    background-color: white; 
  }

  .content {
    text-align: center;
  }


</style>