<template>
  
    <AppHeader :linkData="headerData" />
    <AppMain />
    <AppFooter />

</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import '/src/style/general.scss';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
  data() {
    return {
      headerData: {
        imageLogo: 'imgs/avada-freelance-logo.png',
        url: '#',
        plus: '<i class="fa-solid fa-plus"></i>',
        menu: '<i class="fa-solid fa-bars"></i>'
      }
    };
  }
};
</script>
