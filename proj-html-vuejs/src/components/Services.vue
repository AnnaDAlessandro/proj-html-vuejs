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
    <div class="services">
        <div class="triangle">
          <svg xmlns="http://www.w3.org/2000/svg" class="fusion-big-triangle-candy" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="fill:#ffffff;padding:0;"><path d="M0 100 L50 2 L100 100 Z"/></svg>  
        </div>
       
       <span>meens grooming</span>
      
    </div>

    
</template>

<style scoped>
.services {
    position: relative;
    background-color: white;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .content {
    text-align: center;
  }

  .triangle {
    position: absolute;
    top: -40;
    width: 100%;
    height: 225px;
    z-index: 2;
  }

</style>
