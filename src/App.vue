<template>
  <AppHeader :linkHeaderData="headerData" />
  <AppMain />
  <AppFooter :linkFooterData="footerData" />

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
        url: '#',
        menu: '<i class="fa-solid fa-bars"></i>',
        url: '#',
      },
      footerData: {
        imageLogo: 'imgs/avada-footer-logo.png',
        url: '#',
        copyInfo: '&copy Copyright 2012-2020 | ',
        themeInfo: ' Avada Theme by ',
        privacy: ' | All Rights Reserved |',
        powered: ' Powered by ',

      }
    };
  }
};

</script>
