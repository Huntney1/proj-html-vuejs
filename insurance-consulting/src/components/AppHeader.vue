<script>
export default {
    name: "AppHeader",
  data() {
    return {
      /* lista voci nav-bar */
      menu: [
        {
          label: "Demos",
          url: "#",
          active: false,
        },
        {
          label: "Pages",
          url: "#",
          active: true,
        },
        {
          label: "Potfolio",
          url: "#",
          active: false,
        },
        {
          label: "Blog",
          url: "#",
          active: false,
        },
        {
          label: "Shop",
          url: "#",
          active: false,
        },
      ],
    };
  },
};

</script>

<template lang="">
    <header class="continer">
    <!-- NavBar -->
    <div class="navbar d-flex justify-content-beatween">
      <!-- logo dc -->
      <a href="#" class="logo">
        <img src="/img/nexgen-logo.svg" alt="Logo_NG" />
      </a>
      <!-- attivo lista nav bar -->
      <nav>
        <ul>
          <li v-for="(item, index) in menu" :key="index">
            <a :href="item.url" :class="item.active ? 'active' : ''">
            {{ item.label }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
    
    .navbar {
  
  align-items: center;

  height: 125px;
  margin: 1em 0 0 0;

  nav {
    @include d-flex-cent;
    height: 100%;

    ul {
      height: 100%;
      display: flex;
      list-style: none;

      li {
        height: 100%;
        padding: 10px;
       /*  line-height: 1px; */
       border-bottom: 3px solid white;
        /* transition: border 0.3s; */
        &.active {
          /* color: $primary; */
          border-bottom: 3px solid blue;
          cursor: pointer;

          a {
            color: blue;
          }
        }
        &:hover {
          border-bottom: blue;
        }

        a:hover{
          border-bottom: blue
        }
      }
    }
  }
}
  
</style>