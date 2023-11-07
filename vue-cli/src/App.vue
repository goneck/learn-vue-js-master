<template>
  <div>
    <app-header :headerTitle="str" @renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  data() {
    return {
      str: "Header",
    };
  },
  components: {
    "app-header": AppHeader,
  },
  methods: {
    renewStr() {
      this.str = "hi";
    },
  },
};
</script>

<style></style>
