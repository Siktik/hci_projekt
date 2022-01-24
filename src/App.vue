<template>

  <container>

    <Header/>
    <Navigation/>
<section>
    <KursAnsicht/>
</section>


  </container>

</template>

<script>
autosize(document.querySelector('section'));
import Header from './components/Header';
import KursAnsicht from './components/KursAnsicht';
import Navigation from './components/Navigation'
export default {
  name: 'App',

  components: {
    Header,
    KursAnsicht,
    Navigation,
  },

  data: () => ({
    //
  }),
};
</script>
