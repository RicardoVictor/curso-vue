<template>
  <div>
    <button
      @click="
        firstEvent(firstEventName, $event), secondEvent(secondEventName, $event)
      "
    >
      Activate multiple events
    </button>
    <p>{{ multiple_events }}</p>
  </div>
</template>

<script>
export default {
  name: "MultipleEvents",
  data() {
    return {
      multiple_events: "",
      firstEventName: "First event",
      secondEventName: "Second event",
    };
  },
  methods: {
    firstEvent(eventName, event) {
      this.multiple_events = `Event: '${eventName}' activated!`;
    },
    secondEvent(eventName, event) {
      setTimeout(() => {
        this.multiple_events = `Event: '${eventName}' activated!`;
      }, 1000);
    },
  },
};
</script>

<style scoped>
div {
  margin: 100px;
}
</style>