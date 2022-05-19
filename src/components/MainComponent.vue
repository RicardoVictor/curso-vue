<template>
  <div>
    <Reuse />
    <h1>Hello Vue</h1>
    <p>Creator: {{ name }}, {{ occupation }}</p>
    <Reuse />
    <MultipleEvents />
    <Reuse />
  </div>
</template>

<script>
import MultipleEvents from "./MultipleEvents.vue";
import Reuse from './Reuse.vue';
export default {
  components: {
    MultipleEvents,
    Reuse,
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