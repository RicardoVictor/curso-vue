<template>
  <div>
    <h1>Component name: {{ name }}</h1>
  </div>
</template>

<script>
export default {
  name: "LifeCicle",
  data() {
    return {
      name: "LifeCicle",
    };
  },
  created() {
    setTimeout(() => {
      this.name = "Life Cicle";
    }, 1000);
  },
  mounted() {
    setTimeout(() => {
      this.name = "Life Cicle Component";
    }, 2000);
  },
};
</script>