<template>
  <div>
    <h1>Hello Vue</h1>
    <p>Creator: {{ name }}, {{ occupation }}</p>
    <MultipleEvents />
  </div>
</template>

<script>
import MultipleEvents from "./MultipleEvents.vue";
export default {
  components: {
    MultipleEvents,
  },
  name: "MainComponent",
  data() {
    return {
      name: "Victor",
      occupation: "Dev C#",
    };
  },
};
</script>