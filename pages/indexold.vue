<template>
  <section class="container">
    <div>
      <app-logo/>
      <h1 class="title">
        www.bestgate.sk
      </h1>
      <h2 class="subtitle">
        Ponúkame široký sortiment vysokokvalitných výrobkov zo železa. 
      </h2>
      <div class="links">
        <a
          href="/domov"
          target="_blank"
          class="button--green">Vstúpte</a>
      </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-image: url("/assets/img/index.png");
  background-repeat: no-repeat;
  background-position: center;
  background-attachment: fixed;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  font-weight: 400;
  font-size: 100px;
  color: #35495E;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: white;
  word-spacing: 5px;
  padding-bottom: 15px;

}

.links {
  padding-top: 15px;
}




</style>
