<template>
    <div>
      <button @click="toggleMenu" class="hamburger-menu-button">
        <span></span>
        <span></span>
        <span></span>
      </button>
      <div v-if="showMenu" class="menu">
        <ul>
            <li v-for="(element, index) in ListaMenu" :key="index">
          <a :href="element.href" @mouseover="hoverItem" @mouseout="unhoverItem">
            {{ element.titolo }}
          </a>
        </li>
      </ul>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        ListaMenu:[
            { titolo:"Home",
              href:"#"
            },
            { titolo:"About Us",
              href:"#pro-barber"
            },
            { titolo:"Services",
              href:"#services"
            },
            { titolo:"Shop",
              href:"#products"
            },
            { titolo:"Our Team",
              href:"#reviews"
            },
            { titolo:"Blog",
              href:"#blog"
            },
            { titolo:"Contact Us",
              href:"#contact-us"
            }

        ],
    
        showMenu: false
      }
    },
    methods: {
      toggleMenu() {
        this.showMenu = !this.showMenu;
      },
      hoverItem(event) {
      event.target.style.color = '#BE9359'; 
    },
    unhoverItem(event) {
      event.target.style.color = '#FFFFFF'; 
    },
    },
  };
  </script>
  
  <style scoped>
  .hamburger-menu-button {
    display: flex;
    flex-direction: column;
    cursor: pointer;
    background: none;
    border: none;
    padding: 10px;
  }
  
  .hamburger-menu-button span {
    width: 28px;
    height: 3px;
    background-color: white;
    margin: 5px 0;
  }
  
  .menu {
    position: absolute;
    top: 80px;
    padding: 10px;
    display: flex;
    flex-direction: column;
  }
  
  .menu ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }
  
  .menu li {
    margin-bottom: 10px;
  }
  
  .menu a {
    text-decoration: none;
    color: white;
    font-weight: bold;
  }
  .menu a:hover {
  color:#BE9359; 
}
  </style>