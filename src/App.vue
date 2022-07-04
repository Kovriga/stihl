<template>
  <div id="app">
    <nav-bar/>
    <carousel :sliderItems="sliderItems"></carousel>
  </div>
</template>

<script lang="ts">
import {Component, Vue} from 'vue-property-decorator';
import NavBar from "@/components/NavBar.vue";
import Carousel from "@/components/carousel/Carousel.vue";

@Component({
  components: {Carousel, NavBar},
})
export default class App extends Vue {
  sliderItems: any = [
    {
      image: 'promo-01.png',
      name:'promo-01',
    },
    {
      image: 'promo-02.png',
      name:'promo-02',
    },
  ]
}
</script>

<style lang="sass">
*
  margin: 0
  padding: 0

body, html
  height: 100%

#app
  height: 100%

@font-face
  font-family: 'Montserrat-Bold'
  src: url("assets/fonts/Montserrat-Bold.woff") format('woff')
</style>
