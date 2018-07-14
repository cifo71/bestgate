<template>
    <div>
        <ui-menu/>
        <div class="about">
           
                <ui-layout class="col-xs-12">

                <ui-map/>
              
            </ui-layout>
        </div>
        <ui-footer/>   
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
h1{
color: black;
padding: 40px;

}
</style>