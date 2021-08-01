<template>
    <h1>From Docker</h1>
  Hello {{ name }} welcome to my app.
  <hr />
  <counter></counter>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import Counter from "./Counter.vue";

export default defineComponent({
  components: {
    Counter,
  },
  setup() {
    const name = ref<string>("Bijaya");
    return {
      name,
    };
  },
});
</script>
