<template>
  <div>
    <h2>Formulário:</h2>
    <form action="" @submit="sendForm($event)">
      <div>
        <input type="text" v-model="name" />
      </div>
      <div>
        <input type="text" v-model="email" />
      </div>
      <div>
        <Submit />
      </div>
    </form>
  </div>
</template>

<script>
import InputText from "./form/InputText.vue";
import Submit from "./form/Submit.vue";

export default {
  name: "Form",
  components: {
    InputText,
    Submit,
  },
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    sendForm(event) {
      event.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Sending form...");
      console.log("name: " + name);
      console.log("email: " + email);

      // enviar dados para o servidor aqui.
    },
  },
};
</script>