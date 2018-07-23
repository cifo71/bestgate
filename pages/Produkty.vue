<template>
  <div>
    <div class="products-header">
    </div>
    <ui-menu />
    <ui-layout container>
			<ui-layout class="col-xs-12">
				<div class="products-title"><h1>Produkty</h1></div>
			</ui-layout>
    </ui-layout>
    <div class="body">
    <ui-layout wrap container justify-center>
			<ui-layout class="col-xs-12 col-sm-6 col-md-4">
        <div class="brany">Brány</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6 col-md-4">
        <div class="ploty">Ploty</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6 col-md-4">
        <div class="zabradlia">Zábradlia</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6 col-md-4">
        <div class="schody">Schody</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6 col-md-4">
        <div class="pristresky">Pristresky</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6  col-md-4">
        <div class="postele">Postele</div>
      </ui-layout>
      <ui-layout class="col-xs-12 col-sm-6  col-md-4">
        <div class="ostatne">Ostatne</div>
      </ui-layout>
    </ui-layout>
    </div>
  	<ui-footer />   
  </div> 
</template>

<script>
import UiLayout from '~/components/UiLayout.vue'
import UiMenu from '~/components/UiMenu.vue'
import UiFooter from '~/components/UiFooter.vue'

export default {
  components: {
    UiLayout,
    UiFooter,
    UiMenu
  }
}

</script>

<style>

.products-header{
	width: 100%;
	height: 300px;
	background-image: url("/assets/img/products.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.products-title {
	margin:20px;
	padding-top: 60px;
	position:relative;
}

.products-title::before {
	content: " ";
	background:#5383d3;
	width:10px;
  height:35px;
  left:-20px;
  position:absolute;
}

.products-text {
  padding-bottom: 25px;
  line-height: 26px;


}

.brany {
width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;

}

.ploty {

width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;
}

.zabradlia {
width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;


}
.schody {
width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;
}

.pristresky {

width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;
}

.postele {
width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;

}

.ostatne {
width: 500px;
height :200px;
border: 3px solid black;
margin-top: 20px;

}

</style>