<script >
export default{
    name: 'Services',
    data() {
        return{
          
            
        }
    
    },
}
</script>

<template>
    <div id="services">
        <div class="triangle">
          <svg xmlns="http://www.w3.org/2000/svg" class="fusion-big-triangle-candy" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="fill:#ffffff;padding:0;"><path d="M0 100 L50 2 L100 100 Z"/></svg>  
        </div>

        <div class="d-flex flex-column align-items-center">
          <span class="text-capitalize">means grooming</span>
          <h1>Services</h1>
        </div>      
      </div>
      <div class="d-flex p-5" id="services-1">
        <div class="d-flex flex-column align-items-center">
        <figure>
          <img src="../img/avadabarbers-trimcut-icon-before.png" alt="">
        </figure>
        <h2>Trim & Cut</h2>
        <p class="text-center">Avada Barbers are experts in the lickety split trim and hair cut. Quick but careful and ridiculously good looking. </p>

        </div>
        <div class="d-flex flex-column align-items-center">
        <figure>
          <img src="../img/avadabarbers-washndry-icon.png" alt="">
        </figure>
        <h2>Wash & Dry</h2>
        <p class="text-center">Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurious fashion. </p>

        </div>
        <div class="d-flex flex-column align-items-center">
        <figure>
          <img src="../img/avadabarbers-beardtrim-icon.png" alt="">
        </figure>
       
        <h2>Beard Tidy</h2>
        <p class="text-center">Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers. </p>
      
      

        </div>
        
       

      </div>

        <div class="btn-contenitore">
          <button id="btn-services">READ ABOUT OUR SERVICES </button>

        </div>
</template>

<style scoped>
#services {
    position: relative;
    background-color: white;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .triangle {
    position: absolute;
    top: -40;
    width: 100%;
    height: 534px;
    z-index: 2;
  }
  #services h1{
    color: #B0B0B0;
    font-weight:bold;
    font-size: 80px;
  }
  #services span{
    margin-top: 200px;
    color: #BE9359;
    font-weight: bold;
    font-size: 20px;
  }
#services-1{
  margin: 0 auto;
  width: 80%;
  gap: 150px;
}
#services-1 figure{
  display: block;
  margin-bottom: 30px;
}
#services-1 figure img{
  width:100px;
  height: 130px;
}
#services-1 h2{
  color: #BE9359;
  margin-bottom: 30px;

}
#services-1 p{
  color: #B0B0B0;

}
#btn-services{
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
#btn-services:hover {
            opacity: 0.7;
            font-size:18px;
}
.btn-contenitore {
  text-align: center; 
  display: flex; 
  justify-content: center; 
  align-items: center;
  margin-bottom: 200px;
}

</style>
