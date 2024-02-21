<script >
import Info from './Info.vue';
export default{
    name: 'Footer',
    components: {
    Info
  },
    data() {
        return{
            arrayInfo:[
                {  contact:"Avada Barbers",
                   href:"#"

                },
                {  contact:"123 New York Street ",
                   href:"#"

                },
                {  contact:"New York City",
                   href:"#"

                },
                {  contact:"info@yourwebsite.com ",
                   href:"#"

                },
                {  contact:"+1 (555) 555-1212 ",
                   href:"#"

                }
            ]
            
        }
    
    },
}
</script>

<template>
    <footer> 

           
        <div id="contact-us" class="text-center">
            <img src="../img/avadabarbers-stickylogo-x2.png" alt="logo" class="my-5">
            <div class="d-flex" id="contact-us-2">
             <div >
                <figure>
                    <img src="../img/avadabarbers_footer_shop_image-300x234.png" alt="">
                </figure>
                <div>
                    <button class="btn-footer" >SHOP OUR RANGE NOW </button>
                </div>

            </div>
            <div id="contact-us-3" class="text-center">
              <div>
               <Info
               v-for="(element,index) in arrayInfo"
               :key="index"
               :propsContact="element.contact"
               :propsHref="element.href">
            </Info>
        
              </div>
              <div class="d-flex flex-column align-items-center justify-content-center">
             <h4 class="d-flex align-items-center justify-content-center"> FOLLOW US</h4>
             <div class="d-flex align-items-center justify-content-center gap-3" id="contact-us-4">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-youtube"></i>
            <i class="fab fa-instagram"></i>

            </div>
            </div>
            
            </div>
            <div>
                <figure>
                    <img src="../img/avadabarbers_footer_appointment_image-300x234.png" alt="">
                </figure>
                <div>
                    <button  class="btn-footer">BOOK YOUR APPOINTMENT</button>
                </div>
            </div>
            </div>

        </div>
        <div class="copyright d-flex align-items-center justify-content-center">
            <div class="copyright-2">
                <span class="d-flex align-items-center justify-content-center gap-1">
                <i class="fas fa-copyright"></i> copyright 2012-2020 | avada theme by themeFusion | all right reserved | Powered by wordPress
                </span>
            </div>

            

        </div>
    </footer>
  
</template>

<style scoped>
#contact-us{
   padding: 50px;
    background-color: #121314;
}
.fa-facebook-f,
.fa-twitter,
.fa-instagram,
.fa-youtube{
    color: white;
}
#contact-us-2{
    margin: 0 auto;
    width: 56%;
}
#contact-us-3{
    margin-top: 80px;
}
#contact-us-4{
    margin-top: 20px;
    margin-left: 30px;
}
h4{
    margin-top: 15px;
   margin-left: 30px;
   color: #BE9359;
}
.btn-footer{
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
.btn-footer:hover {
            opacity: 0.7;
            font-size:18px;
}
.copyright{
    background-color: #161718;
    height: 100px;
    
}
.copyright-2{
    margin: 0 auto;
    width: 50%;
}
</style>
