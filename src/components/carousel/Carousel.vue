<template>
  <div class="wrapper">
    <div class="carousel">

      <div class="bg--white">

      </div>
      <div class="bg--orange">

      </div>
      <carousel-item
          v-for="(item, key) in sliderItems"
          :key="key"
          :sliderItem="item">
      </carousel-item>
    </div>
  </div>
</template>

<script lang="ts">
import {Component, Prop, Vue} from "vue-property-decorator";
import CarouselItem from "@/components/carousel/CarouselItem.vue";

@Component({
  components: {CarouselItem}
})

export default class Carousel extends Vue {
  @Prop({type: Object, default: []}) sliderItems!: any

}
</script>

<style lang="sass" scoped>
.wrapper
  height: 100%
  overflow: hidden
  margin: 0 auto

  .carousel
    height: 100%
    display: flex
    align-items: center
    justify-content: flex-end

  .bg--orange
    height: 100%
    width: 631px
    background-color: #d28154

  .bg--white
    height: 100%
    display: flex
    flex: auto
</style>
