<script lang="ts">
import { defineComponent, reactive } from "vue";
import "bootstrap/dist/css/bootstrap.min.css"
import ContentItems from "./components/contentItems.vue"
import ToggleItem from "./components/toggleItem.vue"

export default defineComponent({
  name: "App",
  components: {
    ContentItems,
    ToggleItem
  },
})
</script>

<template>
  <header>
    <div class="wrapper">
      <div>
        title
      </div> 
    </div>
  </header>

  <main>
    <ToggleItem/>
    <ContentItems/>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
