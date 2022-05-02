<template>
  <MeuComponente />
  <LifeCicle />
  <Pessoa />
</template>

<script>
import MeuComponente from "./components/MeuComponente.vue";
import LifeCicle from "./components/LifeCicle.vue";
import Pessoa from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    MeuComponente,
    LifeCicle,
    Pessoa,
  },
};
</script>