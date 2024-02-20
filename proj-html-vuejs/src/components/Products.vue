<script >
    
export default{
    name: 'Products',
    data() {
        return{
           
            
        }
    
    },
    mounted() {
    console.log(this.items);
  },
}
</script>

<template>

        
        <div id="products">
        <div class="triangle-1">
          <svg xmlns="http://www.w3.org/2000/svg" class="fusion-big-triangle-candy" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="fill:#121314;padding:0;"><path d="M0 100 L50 2 L100 100 Z"/></svg>  
        </div>
        <div class="text-center mb-5">
          <span>WE HAVE YOU COVERED </span>
         <h1>Avada Grooming Products</h1>  
        </div>
        <div class="d-flex" id="products-1">
        <div class="d-flex flex-column align-items-center">
            <figure>
                <img src="../img/brush_dark-200x200.png" alt="">
            </figure>
            <h2>Brush</h2>
            <span>$15.00</span>

        </div>
        <div class="d-flex flex-column align-items-center">
            <figure>
                <img src="../img/scissors-200x200.png" alt="">
            </figure>
            <h2>Scissor</h2>
            <span>$85.00</span>

        </div>
        <div class="d-flex flex-column align-items-center">
            <figure>
                <img src="../img/hot_oil_dark-200x200.png" alt="">
            </figure>
            <h2>Hot Oil</h2>
            <span>$15.00</span>

        </div>
        <div class="d-flex flex-column align-items-center">
            <figure>
                <img src="../img/straight_razor_dark-200x200.png" alt="">
            </figure>
            <h2>Straight Razor</h2>
            <span>$30.00</span>

        </div>
        
        </div>
        <div class="btn-contenitore-1">
            <button class="btn-products">SHOP OUR PRODUCT RANGE</button>
        </div>
        <div class="spazio">

        </div>
         
        </div>
    
            <div class="contenitore-2">
              <div id="butter" class="text-start d-flex">
                <figure class="d-flex align-items-center">
                    <img src="../img/shaving_butter-400x400.png" alt="">
                </figure>
                <div class="d-flex flex-column p-4 text-start" id="text-butter">
                    <span class="my-3 ">THIS MONTHS FEATURED PRODUCT</span>
                    <h1 class="my-3 ">SHAVING BUTTER</h1>
                    <p class="my-3">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pel lentesque laoreet enim est, vel molestie dolor ultrices ut. 
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <button class="my-3 w-50" id="btn-butter"> BUY NOW</button>
                </div>

              
            </div> 
           
            </div>
      
        

  
</template>

<style scoped>
#products{
    background-image: url(../img/avadabarbers-reviewsbackground.jpg);
    background-repeat: repeat;
    background-size: cover;
    background-position: top;
    position: relative;
    margin-bottom: 50px;
}
#products h1{
    margin-top: 30px;
    color:  #B0B0B0;
}
.triangle-1{
    position: absolute;
    top:-100px;
    width: 100%;
    z-index: 1;
  }
  #products-1{
    margin: 0 auto;
    width: 80%;
    margin-top: 80px;
  }
  #products-1 figure{
    display: block;
  }
  #products-1 img{
    height: 300px;
    width: 300px;
  }
  #products span,
  #products-1 span,
  #products-1 h2{
    color: #BE9359;
    margin-top: 10px;
  }
  #products-1 span{
    margin-bottom: 50px;
  }
  .btn-products{
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
.btn-products:hover {
            opacity: 0.7;
            font-size:18px;
}
.btn-contenitore-1 {
  text-align: center; 
  display: flex; 
  justify-content: center; 
  align-items: center;
}
.spazio{
    height: 150px;
}
#butter{
    position: absolute;
    z-index: 1;
    top:-100px;
    background-color: #121413;
    border-top: 3px solid #BE9359;
}
.contenitore-2{
    position: relative;
    margin: 0 auto;
    width: 70%;
}
.contenitore-2 figure{
    background-image: url(../img/avadabarbers-cta-background.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    margin: 0 0 0;

}
#text-butter{
    margin: 30px;
}
#text-butter span{
    color: #BE9359;
}
#text-butter h1,
#text-butter p{
    color: #B0B0B0;
}
#btn-butter{
            margin-top: 10px;
            display: inline-block;
            padding: 10px 30px;
            text-align: center;
            text-decoration: none;
            color: #BE9359;
            border: 2px solid #BE9359;
            transition: opacity 0.3s ease;
            background: none;
            text-transform: uppercase;
        } 
#btn-butter:hover {
            opacity: 0.7;
            font-size:18px;
}
#reviews{
    margin-top: 500px;
}

  </style>