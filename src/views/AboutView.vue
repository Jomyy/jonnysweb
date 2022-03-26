<template>
  <p>{{ title }}</p>
</template>
<script>
import { reactive } from "@vue/reactivity";

export default {
  setup() {
    const title = reactive("hallo");
  },
};
</script>
