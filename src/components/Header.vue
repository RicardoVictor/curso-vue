<template>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Projetos</a></li>
    <li><a href="#">Contato</a></li>
  </ul>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
ul {
  list-style: none;
  display: flex;
  background: #777;
}

li {
  margin-right: 10px;
}

a {
  color: #ddd;
  text-decoration: none;
  transition: 0.3s;
}

a:hover {
  color: turquoise;
}
</style>