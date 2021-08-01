<template>
  <button @click.prevent="decrement">-</button>
  {{ count }}
  <button @click.prevent="increment">+</button>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "counter",
  setup() {
    const count = ref<number>(0);
    const increment = (): number => {
      return count.value++;
    };
    const decrement = (): number => {
      return count.value--;
    };
    return {
      count,
      increment,
      decrement,
    };
  },
});
</script>
