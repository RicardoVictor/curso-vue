<template>
  <div>
    <h2>Name: {{ name }}</h2>
    <Info />
  </div>
</template>

<script>
import Info from './Info.vue'

export default {
  name: "Pessoa",
   components: {
     Info
   },
  data() {
    return {
      name: "Ricardo Victor",
    };
  },
};
</script>