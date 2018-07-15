<template>
      <header class="menu">
      <router-link :to="{ name: 'index' }">
        <h3>www.bestgate.sk</h3>
      </router-link>
      <nav>
        <router-link :to="{ name: 'index' }">Domov</router-link> 
        <router-link :to="{ name: 'o-nas' }">O nás</router-link> 
        <router-link :to="{ name: 'produkty' }">Produkty</router-link> 
        <router-link :to="{ name: 'kontaktujte-nas' }">Kontaktujte nás</router-link>
      </nav>
    </header>
</template>

<script>

</script>

<style lang="scss">
@import "~@/assets/scss/reset";
@import "~@/assets/scss/variables";
@import "~@/assets/scss/mixins";

.menu {
  width:           100%;
  height:          40px;
  background:      #292C2F;
  padding:         0 40px;
  display:         flex;
  align-items:     center;
  justify-content: space-between;
  top:             200px;
  left:            0;
  position:        absolute;
  
  

  h3 {
    color: white;
  }

  nav {
    display: none;
    @include media(md) {
    display: flex;
    }
    
    a {
      padding:   12px;
      color:     $accent;
      font-size: 18px;
      display:   block;

      &:not(:last-of-type) {
        margin-right: 60px;
      }
      
      &:hover {
        color: $primary;
      }
    }
  }
}
</style>
