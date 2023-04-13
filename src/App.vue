<script>
  import AppHeader from "./components/AppHeader.vue";
  import HeaderBottom from "./components/HeaderBottom.vue";
  import HeaderIcons from "./components/HeaderIcons.vue";
  import AppFooter from "./components/AppFooter.vue";


  export default {
    components: { AppHeader, HeaderBottom, HeaderIcons, AppFooter
     }
    
}
</script>

<template>
  <AppHeader />
  <HeaderBottom />
  <HeaderIcons />
  <AppFooter />
</template>

<style lang="scss">
  @use "../src/assets/style/general.scss"

</style>