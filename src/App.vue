<script>
import TheHeader from "./components/TheHeader.vue"
import TheMain from "./components/TheMain.vue"
import TheFooter from "./components/TheFooter.vue"
import BarraSottoNav from "./components/BarraSottoNav.vue"
import Jumbotron from "./components/Jumbotron.vue"


export default {
  components: { TheHeader, TheMain, TheFooter, BarraSottoNav, Jumbotron},

  data() {
    return {

    };
  },
  methods: {},

  beforeMount() { },
}
</script>


<template>
  <div class="">
    <div>
      <TheHeader class="container"></TheHeader>
    </div>
    <div class="background-nav-inf d-flex align-items-center ">
      <BarraSottoNav class="container"></BarraSottoNav>
    </div>
    <div class="background-card">
      <TheMain class="container"></TheMain>
    </div>
    <div class="background-jumbotron">
      <Jumbotron class="container"></Jumbotron>
    </div>
    <div>
      <TheFooter class="container"></TheFooter>
    </div>
  </div>

</template>

<style lang="scss">
@use "./styles/general.scss";
</style>