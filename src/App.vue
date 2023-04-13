<script>
  import AppHeader from "./components/AppHeader.vue";
  import HeaderBottom from "./components/HeaderBottom.vue";


  export default {
    components: { AppHeader, HeaderBottom }
    
}
</script>

<template>
  <AppHeader />
  <HeaderBottom />
</template>

<style lang="scss">
  @use "../src/assets/style/general.scss"

</style>