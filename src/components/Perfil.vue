<template>
  <div>
    <h2>Name: {{ name }}</h2>
    <Info />
    <Form />
  </div>
</template>

<script>
import Info from "./Info.vue";
import Form from "./Form.vue";

export default {
  name: "Perfil",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      name: "Ricardo Victor",
    };
  },
};
</script>