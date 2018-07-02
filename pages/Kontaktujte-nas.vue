<template>
    <div>
        <ui-header/>
            <ui-layout container>
                <ui-layout class="col-xs-6 col-md-3"></ui-layout>
                <ui-layout class="col-xs-6 col-md-3"></ui-layout>
            </ui-layout>
        <ui-footer/>   
    </div> 
</template>

<script>
import UiHeader from '~/components/UiHeader.vue'
import UiFooter from '~/components/UiFooter.vue'

export default {
  components: {
    UiHeader,
    UiFooter
  }
}

</script>

<style>

</style>