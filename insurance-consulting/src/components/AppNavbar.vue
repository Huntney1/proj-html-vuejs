<script>
export default {
  props: {
    menu: Array,
  },
  data() {
    return {};
  },
};
</script>

<template lang="">
  <nav>
    <ul class="nav nav-list">
      <li
        v-for="(item, index) in menu"
        :key="index"
        :class="item.active ? 'active' : ' '"
        class="nav-item lista"
      >
        <div class="dropdown_">
          <div class="dropbtn">
            <a
              :href="item.url"
              :class="item.active ? 'active' : ' '"
              class="menuitem"
            >
              {{ item.label }}
            </a>
          </div>
          <div class="dropdown_content">
            <a v-for="(item, index) in item.sublabel" :key="index" href="#">
              {{ item }}
            </a>
          </div>
        </div>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss">
  ul {
      display: flex;
      text-decoration:none;
      list-style: none;
    
        li {
            /* height: 100%; */
            padding: 10px;
            line-height: 1px;
        a{
            text-decoration:none;
            color: #e2e3e7;
        }
        }
    }
.menuitem {
  font-size: 15px;
  font-weight: 600;
  text-decoration: none;
 
}
.menuitem:hover {
  color: #132e43;
}

.dropbtn {
  color: #fff;
  padding: 16px;
  font-size: 16px;
  border: none;
}
.dropdown {
  position: relative;
  display: inline-block;
}
.dropdown_content {
  display: none;
  position: absolute;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
  background-color: black;
  min-width: 250px;
  padding: 30px 15px;
}
.dropdown_content a {
  color: grey;
  padding: 6px 16px;
  text-decoration: none;
  display: block;
}
.dropdown_content a:hover {
  color: white;
}
.dropdown_:hover .dropdown_content {
  display: block;
}
</style>