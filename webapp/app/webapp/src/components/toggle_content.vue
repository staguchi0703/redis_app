<template>
  <div>
    <button onclick="al">
      <Toggle v-model="value" />
      <div>toggle switch</div>
    </button>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import Toggle from "@vueform/toggle";
// import * as IORedis from 'ioredis';

export default defineComponent({
  components: {
    Toggle,
  },
  data() {
    return {
      value: true,
    };
  },
  methods: {
    al: ()=>{
      alert()
    },
  }
  });

// method() {
//   ToggleVal: ()=>{
//     const redis = new IORedis("localhost", 6379);
//     redis.sadd("toggleKey", this.value);
//   }
// }
</script>

<style src="@vueform/toggle/themes/default.css"></style>