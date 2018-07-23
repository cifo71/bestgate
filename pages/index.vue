<template>
  <div>
  <ui-header/>
    <div class="index-body">
    <ui-layout column align-center>
    <ui-layout class="col-xs-12">
      <h1 class="index-title">Ponúkame široký sortiment vysokokvalitných výrobkov zo železa!</h1>
    </ui-layout>
    <ui-layout class="col-xs-12">
      <div class="index-button--white"><router-link :to="{ name: 'o-nas' }">Vstúpte</router-link></div>
    </ui-layout>
    </ui-layout>
    </div>
  <ui-footer/>   
  </div>
</template>



<script>
import UiLayout from '~/components/UiLayout.vue'
import UiHeader from '~/components/UiHeader.vue'
import UiFooter from '~/components/UiFooter.vue'

export default {
  components: {
    UiLayout,
    UiHeader,
    UiFooter
  }
}
</script>

<style lang="scss">
@import "~@/assets/scss/reset";
@import "~@/assets/scss/variables";
@import "~@/assets/scss/mixins";

.index-body {
  min-height: calc(100vh - 42px);
  background-image: url("/assets/img/index.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.index-title {
  font-weight: 400;
  font-size: 60px;
  color: white;
  text-shadow: -2px 0 black, 0 2px black, 2px 0 black, 0 -2px black;
  letter-spacing: 1px; 
  padding-top: 180px;
  margin: 10px;
  text-align: center;
}


.index-button--white {
  display: inline-block;
  height: 40px;
  border-radius: 40px;
  border: 3px solid #292C2F;
  color: #292C2F;
  background-color: white;
  text-decoration: none;
  padding: 10px 25px;
  margin: 40px;
}

.index-button--white:hover {
  color: #292C2F;
  background-color: #E4EADE;
  border-radius: 40px;
  border: 3px solid white;
}






@media screen and (max-width: 900px){
   
  .index-title{

    font-size: 46px;
  }
  }

@media screen and (max-width: 800px){
   
  .index-title{

    font-size: 42px;
  }
  }

@media screen and (max-width: 600px){
   
  .index-title{

    font-size: 32px;
  }
  }
</style>