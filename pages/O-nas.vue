<template>
    <div>
        <ui-menu/>
            <ui-layout container>
            </ui-layout>
        <ui-footer/>   
    </div> 
</template>

<script>
import UiHeader from '~/components/UiHeader.vue'
import UiMenu from '~/components/UiMenu.vue'
import UiFooter from '~/components/UiFooter.vue'

export default {
  components: {
    UiHeader,
    UiFooter,
    UiMenu
  }
}

</script>

<style>

</style>