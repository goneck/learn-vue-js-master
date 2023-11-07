<template>
  <header>
    <h1>{{ headerTitle }}</h1>
    <button @click="sendEvent">send</button>
  </header>
</template>

<script>
export default {
  props: ["headerTitle"],
  methods: {
    sendEvent() {
      this.$emit("renew");
    },
  },
};
</script>

<style></style>
