<template>
  <div class="carousel-item">
  </div>
</template>

<script lang="ts">
import {Component, Prop, Vue} from "vue-property-decorator";

@Component

export default class CarouselItem extends Vue{
  @Prop({ type: Object, default: []}) sliderItem!: any
}
</script>

<style lang="sass" scoped>
</style>
