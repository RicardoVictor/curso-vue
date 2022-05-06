<template>
  <div>
    <h2>Info</h2>
    <div v-if="is_working">
      <p>I'm currently employed.</p>
      <p>Working at: {{ company }}</p>
    </div>
    <div v-else>
      <p>I'm open to work.</p>
    </div>
    <button @click="showEmail">{{ button_email_text }}</button>
    <div v-show="show_email">
      <p>Send a message to: {{ email }}</p>
    </div>
    <p>Skills:</p>
    <ul>
      <li v-for="skill in skills" :key="skill">{{ skill }}</li>
    </ul>
    <p>To access portfolio: <a :href="portfolio_link">click here</a>.</p>
    <Picture />
  </div>
</template>

<script>
import Picture from "./Picture.vue";
export default {
  components: { Picture },
  name: "Info",
  data() {
    return {
      is_working: true,
      show_email: true,
      company: "Dell Lead",
      email: "user@gmail.com",
      skills: ["C#", "SQL", "Git"],
      portfolio_link: "https://google.com",
      button_email_text: "Hide email",
    };
  },
  methods: {
    showEmail() {
      this.show_email = !this.show_email;
      if (this.show_email) this.button_email_text = "Hide email";
      else if (!this.show_email) this.button_email_text = "Show email";
    },
  },
};
</script>