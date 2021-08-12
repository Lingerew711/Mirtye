<template>
<div class="container-fluid">
  <v-app>
    <Topnav title="Products"/>

  <Body/>

  <Footer/>
  </v-app>
</div>
</template> 

<script>
import Topnav from './components/topnav/Topnav'
import Footer from './components/footer/Footer'
import Body from './components/body/Body'
export default {
  name: 'App',
  components: {
    Topnav,
    Body,
    Footer,
  },
}
</script>

<style>
@import url("assets/css/footer.css");
@import url("assets/css/topnav.css");
@import url("assets/css/body.css");
@import url("assets/css/search.css");
</style>
