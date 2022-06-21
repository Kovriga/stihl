<template>
  <div id="app">
    <nav-bar/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import NavBar from "@/components/NavBar.vue";

@Component({
  components: {NavBar},
})
export default class App extends Vue {

}
</script>

<style lang="sass">
*
  margin: 0
  padding: 0

</style>
