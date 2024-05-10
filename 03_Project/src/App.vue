<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: "App",
  component: {},

  data() {
    return {
      score: 1
    }
  }
})
</script>


<template>
  <div>
    <h1>Youre Score is : {{ score }}</h1>

  </div>
</template>
