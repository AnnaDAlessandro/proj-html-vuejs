<script >
export default{
    name: 'Info',
    props:{
        propsContact:String,
        propsHref:String

    },
   
    data() {
        return{
            
        }
    
    },
}
</script>

<template>
       <ul>
       <li><a :href="propsHref">{{ propsContact }}</a></li>
      </ul>
      


</template>



<style scoped>

ul{
   
    list-style-type: none;
}
a{
    text-decoration: none;
    color:#69615b ;
}




</style>