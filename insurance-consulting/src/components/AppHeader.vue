<script>
import AppNavbar from "./AppNavbar.vue"

export default {
  name: "AppHeader",
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
    components:{
      AppNavbar,
    }
};

</script>

<template lang="">
  <header>
    <!-- NavBar -->
    <nav>
      <div class="navbar navbar-expand-lg">

        <!-- logo NG -->
        <div class="col-3">
          <a  href="#" class="navbar-brand">
            <img src="/img/nexgen-logo.svg" alt="Logo_NG" />
          </a>
        </div>

          <!-- richiamo la lista alla nav bar -->        
        <AppNavbar :menu="menu"></AppNavbar>

        <!-- icone -->
        <div class="icon-head">
         <i class="bi bi-search"></i>
          <i class="bi bi-handbag"></i>
        </div>
      </div>
    </nav> 
  </header>
</template>

<style lang="scss" scoped>

    



header{
  background-color: #12565c;
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

    .icon-head{
      color:white;
    }


   /*  ul {
      height: 100%;
      text-decoration:none;

      list-style: none;
    
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