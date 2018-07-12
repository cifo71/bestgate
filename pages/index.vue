<template>
  <div class="index">
  <ui-header/>
    <div class="body">
    <ui-layout column align-center>
    <ui-layout class="col-xs-12">
      <h1 class="title">www.bestgate.sk</h1>
    </ui-layout>
    <ui-layout class="col-xs-12">        
      <h2 class="subtitle">Ponúkame široký sortiment vysokokvalitných výrobkov zo železa.</h2>
    </ui-layout>
    <ui-layout class="col-xs-12">
      <div class="button--green"><router-link :to="{ name: 'domov' }">Vstúpte</router-link></div>
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



.body {
  min-height: calc(100vh - 40px);
  background-image: url("/assets/img/index3.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  font-weight: 400;
  font-size: 100px;
  color: white;
  letter-spacing: 1px; 
  padding-top: 110px;
  margin: 20px;
  text-decoration: underline;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #3B8070;
  word-spacing: 5px;
  padding-bottom: 15px;
  text-align: center;
  padding: 5px;
  background-color: white;
  border-radius: 10px;
  border: 3px solid #3b8070;
}

.button--green {
  display: inline-block;
  height: 40px;
  border-radius: 4px;
  border: 1px solid white;
  color: #fff;
  background-color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
  margin: 30px;
  
}

.button--green:hover {
  color: #fff;
  background-color: #41B883;
}


</style>