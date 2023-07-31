<template>
  <div id="app">
    <RespNavBar
		:nav-links="navLinks"
    :image-path="require('./assets/n1rush.png')"
		background="#000"
		link-color="#FFF"
		hoverBackground="#01b9fa"
    />
    <SliderNav />
  </div>
</template>

<script>
  import RespNavBar from '@/components/RespNavBar.vue'
  import SliderNav from '@/components/SliderNav.vue'

  export default {
    components: { RespNavBar, SliderNav },
    data: () => ({
      navLinks: [
        {
          text: 'Contato',
          path: '/contato',
          icon: 'mdi-alert'
        },
        {
          text: 'Buscar',
          path: '/buscar',
          icon: 'v-icon mdi-plus'
        },
        {
          text: '',
          path: '/loja',
          icon: 'android-icon'
        }
      ]
    })
  }
</script>

<style lang="scss">

@import 'vue-material-design-icons/styles.css';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-block-start: 0%;
  padding-left: 0%;
}

nav {
  padding: 30px;

}
</style>
