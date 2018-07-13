<template>
<div>
<head><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"></head>
  <header class="header">
    <ui-layout class="col-xs-12" justifyStart>
      <router-link :to="{ name: 'index' }"><h3>www.bestgate.sk</h3></router-link>   
    <ui-layout justifyEnd>
     <div class="header-info">
				<div>
					<i class="fa fa-map-marker"></i>
					Horná Krupá, Slovensko
					<i class="fa fa-phone"></i>
					+1 555 123456
					<i class="fa fa-envelope"></i>
					info@bestgate.sk
				</div>
			</div>
    </ui-layout>
    </ui-layout>
  </header>
</div>
</template>

<script>
import UiLayout from '~/components/UiLayout.vue'

export default {
  components: {
    UiLayout
  }
}
</script>

<style lang="scss">
@import "~@/assets/scss/reset";
@import "~@/assets/scss/variables";
@import "~@/assets/scss/mixins";

.header {
  width: 100%;
  height: 42px;
}
  
.header-info i {
	background-color:  #33383b;
	color: #ffffff;
	font-size: 25px;
	width: 36px;
	height: 36px;
	border-radius: 50%;
	text-align: center;
	line-height: 42px;
  margin: 3px;
}

h3 {
  font-size: 25px;
  padding: 9px;
}
</style>
