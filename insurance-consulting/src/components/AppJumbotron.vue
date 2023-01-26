<script>
import AppPrompt from "./AppPrompt.vue";
export default {
  name:'AppJumbotron',
  components:{
    AppPrompt,
  }

};
   
</script>

<template lang="">
    <div>
        <div class="jumbotron">
          <AppPrompt />
        </div>
    </div>
    
</template>

<style lang="scss" scoped>
.jumbotron {
  background-image: url("../../public/img/bg-6.jpg");
  background-position: center;
  background-size: cover;
  height: 26em;
  /* width: 10em; */
}
</style>
