<template>
  <Header />
  <MainComponent />
  <LifeCicle />
  <Perfil />
</template>

<script>
import Header from "./components/Header.vue";
import MainComponent from "./components/MainComponent.vue";
import LifeCicle from "./components/LifeCicle.vue";
import Perfil from "./components/Perfil.vue";

export default {
  name: "App",
  components: {
    Header,
    MainComponent,
    LifeCicle,
    Perfil,
  },
};
</script>

<style>
body {
  background-color: #333;
  color: #fff;
}
</style>