<script>
import AppNavbar from "./AppNavbar.vue";
import AppJumbotron from "./AppJumbotron.vue";

export default {
  name: "AppHeader",
  
  components:{
    AppNavbar,
    AppJumbotron,
    },

  data() {
    return {
      menu: [
        {
          label: "Demos",
          url: "#",
          active: false,
          sublabel: [
            'Home 1',
            'Home 2',
            'Home 3',
            'Home 4',
            'Home 5',
            'Home 6',
            'Home 7',
            'Home 8',
            'Home 9',
            'Home 10',
            'Home 11',
            'Leverage',
          ] 
        },
        {
          label: "Pages",
          url: "#",
          active: true,
          sublabel: [
            "About Us",
            "Service",
            "Single Service",
            "Pricing Table",
            "Testimonials",
            "Team",
            "Partners",
            "Contact Us",
          ],
        },
        {
          label: "Potfolio",
          url: "#",
          active: false,
          sublabel:[
            'Full Width',
            'With Sidebar',
            'Single Portfolio',
        ],
      },
        {
          label: "Blog",
          url: "#",
          active: false,
          sublabel:[
            'Full Width',
            'With Sidebar',
            'Single Post',
          ]
        },
        {
          label: "Shop",
          url: "#",
          active: true,
        },
      ],
    };
  },
    
};

</script>

<template lang="">
  
  <header>
    
    <!-- NavBar -->
    <nav>
      <div class="navbar navbar-expand-lg">

        <!-- logo NG -->
        <div class="col-12">
          <a  href="#" class="navbar-brand">
            <img src="/img/nexgen-logo.svg" alt="Logo_NG" />
          </a>
        </div>

          <!-- richiamo la lista alla nav bar -->        
        <AppNavbar :menu="menu"></AppNavbar>

        <!-- icone -->
        <div class="icon-head">
         <i class="bi bi-search "></i>
          <i class="bi bi-handbag"></i>
        </div>

        <!-- bottone -->
        <div>
          <li class="nav-item">
            <button type="button" class="head-button">BUY NEXGEN</button>
          </li>
        </div>
      </div>
    </nav> 
    <AppJumbotron />
  </header>
</template>

<style lang="scss" scoped>
 @use "../style/partials/variables" as *;
    

header{
  background-color: $blue-primary;
  width: 100%;
}
.navbar {
  
    /* height: 125px; */
    display: flex;
    justify-content: space-around;
    align-items: center;

   img {
      width: 100px;
    }

    .nav-item{
      list-style: none;
       text-decoration:none;
    }

    .bi-search{
      margin: 1em;
    }

    .icon-head{
      color:white;
      margin-right: 2em;
    }


    .head-button{
      width: 13em;
      height: 3.5em;
      background-color: $black-primary;
      border: 2px solid $blue-third;
      border-radius: 2.5em;
      color: $grey-secondary;
    }

   /*  ul {
      height: 100%;
     

      
    
      li {
        height: 100%;
        padding: 10px;
        line-height: 1px;
        color:#fff;
                
        a{
          text-decoration:none;
          color: #fff;
        }
        
   
    }
  } */
}
</style>