<template>
  <div>
    <div class="about-header">
    </div>
    <ui-menu />
    <ui-layout container column>
			<ui-layout class="col-xs-12">
				<div class="about-title"><h1>O nás</h1></div>
			</ui-layout>
			<ui-layout class="col-xs-12">
        <div class="about-text">
	       <p>Text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text.
          Text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text.
        	Text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text.
          Text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text text.</p>
        </div>
      </ui-layout>
    </ui-layout>
                
    <ui-layout container>      
    <ui-layout class="col-xs-12">
      <ui-map />
    </ui-layout>
		</ui-layout>
  	<ui-footer />   
  </div> 
</template>

<script>
import UiLayout from '~/components/UiLayout.vue'
import UiMenu from '~/components/UiMenu.vue'
import UiFooter from '~/components/UiFooter.vue'
import UiMap from '~/components/UiMap.vue'

export default {
  components: {
    UiLayout,
    UiFooter,
    UiMenu,
    UiMap
  }
}

</script>

<style>

.about-header{
	width: 100%;
	height: 300px;
	background-image: url("/assets/img/about.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.about-title {
  margin:20px;
  padding-top: 60px;
  position:relative;
}

.about-title::before {
  content: " ";
  background:#5383d3;
  width:10px;
  height:35px;
  left:-20px;
  position:absolute;
}

.about-text {
  padding-bottom: 25px;
  line-height: 26px;


}




</style>