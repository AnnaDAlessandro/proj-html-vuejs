<script >
export default{
    name: 'Blog',
    data() {
        return{
            arrayBlog:[
                { image:"Salon-brush.jpg",                 
                  testo:" Lorem ipsum dolor sit amet, consectetur adipiscing el it. Phasellus ut dapibus magna. Praesent semper,",
                  titolo:"Avada Barbers Now Open"
                },
                { image:"salon.jpg",                 
                  testo:" Lorem ipsum dolor sit amet, consectetur adipiscing el it. Phasellus ut dapibus magna. Praesent semper,",
                  titolo:"Choosing The Right Barber"
                },
                { image:"barber.jpg",                 
                  testo:" Lorem ipsum dolor sit amet, consectetur adipiscing el it. Phasellus ut dapibus magna. Praesent semper,",
                  titolo:"Quick Service Guide"
                }
            ]
            
        }
    
    },
}
</script>

<template>
    <div id="blog">
        <svg xmlns="http://www.w3.org/2000/svg"
     class="fusion-big-triangle-candy"
     version="1.1"
     width="100%"
     height="100"
     viewBox="0 0 100 100"
     preserveAspectRatio="none"
     style="display: block; fill:#FFFFFF; padding:0;">
  <path d="M0 100 L50 2 L100 100 Z" transform="rotate(180, 50, 50)"/>
</svg>
      <div class="text-center my-5" id="blog-1">
        <span>TALES FROM THE BARBER SHOP </span>
        <h1>Recent Blog Posts </h1>
      </div>
       
       <div class="d-flex text-center" id="blog-2">
        <div class="text-center"
        v-for="(element,index) in arrayBlog"
        :key="index">
            <img :src="`/src/assets/${element.image}`" alt="" style="width:350px; height: 230px;">
            <h3 class="my-3">{{ element.titolo }}</h3>
            <p class="my-4">{{ element.testo }}</p>
        </div>
       </div>

        <div class="btn-contenitore-2">
        <button class="btn-blog">READ MORE FROM OUR BLOG</button>
       </div>
       
       

       
        
       
    </div>
  
</template>

<style lang="scss" scoped>
#blog{
    background-color: #f5f5f5;

}

#blog-1 span{
    font-size: 24px;
    font-weight: bold;
    color:  #BE9359;
}
#blog-1 h1{
    margin-bottom: 100px;
    font-size: 80px;
    color: #b0b0b0;
}
#blog-2{
    margin: 0 auto;
    width: 80%;
   
}
#blog-2 h3{
    font-weight: bold;
    color:  #BE9359;
    margin-inline: 50px;
}
#blog-2 p{
 color: #b0b0b0;
 margin-inline: 60px;

}
.btn-blog{
            margin-top: 60px;
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
            margin-bottom: 100px;

}
.btn-blog:hover {
            opacity: 0.7;
            font-size:18px;
}
.btn-contenitore-2 {
  text-align: center; 
  display: flex; 
  justify-content: center; 
  align-items: center;
}

</style>
