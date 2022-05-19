<template>
  <div>
    <button @click="activate">Clique aqui para mudar ativação independente!</button>
    <span v-show="active">Ativado!</span>
  </div>
</template>

<script>
export default {
  name: "Reuse",
  data() {
    return {
      active: false,
    };
  },
  methods: {
    activate() {
      this.active = !this.active;
    },
  },
};
</script>
