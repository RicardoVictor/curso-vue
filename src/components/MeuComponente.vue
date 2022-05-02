<template>
  <div>
    <h1>Hello Vue</h1>
    <p>Creator: {{ name }}, {{ occupation }}</p>
  </div>
</template>

<script>
export default {
  name: "MeuComponente",
  data() {
    return {
      name: "Victor",
      occupation: "Dev C#",
    };
  },
};
</script>