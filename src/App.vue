<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import AppShop from './components/AppShop.vue';

  export default{
    components:{
      AppHeader,
      AppMain,
      AppShop,
      AppFooter,

    }
  }
</script>

<template>
    <AppHeader />
    <AppMain />
    <AppShop />
    <AppFooter />

</template>


<style lang="scss">
@use "./styles/general.scss";


</style>