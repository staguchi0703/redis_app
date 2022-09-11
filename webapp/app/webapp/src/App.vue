<template>
  <div>
    <Header msg="Welcome redis-sever Gui"/>
    <div class="border border-secondary rounded shadow-lg container">
        <ToggleItem />
        <ViewItems />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Header from './components/header.vue';
import ToggleItem from './components/toggle_content.vue';
import ViewItems from './components/view_contents.vue';
import "bootstrap";
import "bootstrap/dist/css/bootstrap.min.css";

export default defineComponent({
  name: 'App',
  components: {
    Header,
    ToggleItem,
    ViewItems
  }
});
</script>

<style>
</style>
