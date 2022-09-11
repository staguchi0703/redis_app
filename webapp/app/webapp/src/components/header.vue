<template>
  <div class="bg-black">
    <h1 class="text-white">{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: String,
  },
});
</script>


<style scoped>
</style>
