<script >
export default{
    name: 'Reviews',
    data() {
        return{
            items:[
                {
                    testo:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu. ",
                    name:"John Doe",
                    image:"john-doe.jpg"
                },
                {
                    testo:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu. ",
                    name:"Pete Jones",
                    image:"pete-jones.jpg"
                },
                {
                    testo:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu. ",
                    name:"Mark Wilson",
                    image:"Mark-wilson.jpg"
                },
            ]
    
        }
    
    },
}
</script>

<template>
    <div id="reviews">
        <div class="text-center my-5">
            <span class="my-3 text-uppercase">What People Say</span>
                <h1 class="my-3">Reviews</h1>
        </div>
        
                <div class="d-flex text-center" id="single-card">
                   <div class="d-flex flex-column gy-5" v-for="(item, index) in items" 
                :key="index">

                  <p class="">{{ item.testo }}</p>
                 
                  <img :src="`/src/assets/${item.image}`" style="width: 50px; height:50px; border-radius:25px;"  >  
                  <span class="my-5">{{ item.name }}</span>
                     
                 
                 
        </div> 
                </div>
      
    </div>
  
</template>

<style scoped>
#reviews{
    margin-top: 450px;
}
#reviews span,
#single-card span{
    color: #BE9359;
    font-weight: bold;
}
#reviews h1{
    font-weight:bold ;
    color:  #B0B0B0;

}
#single-card{
   margin: 0 auto;
   width: 70%;
   padding: 10px;
   gap: 70px;
}
#single-card span{
    margin-block: 20px;
}
#single-card p{
    margin-block: 30px;
    width: 300px;
}

#single-card img{
    margin: 0 auto;
}


</style>
