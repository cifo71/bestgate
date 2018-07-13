<template>
    <div class="index">
        <ui-menu/>
        <div class="body">
            <ui-layout container>
                <ui-layout class="col-xs-12"><h1>O nás</h1>

                </ui-layout>    
            </ui-layout>
        </div>
        <ui-footer/>   
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
h1{
color: black;
padding: 40px;

}
</style>