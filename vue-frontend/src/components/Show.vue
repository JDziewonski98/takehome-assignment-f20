<template>
  <!-- PART 4: Add your code here -->
  <div>
    {{name}}
    <Counter
    v-bind:epsSeen="this.episodes_seen"/>
  </div>
</template>

<script>
// PART 4: Add your code here
import Counter from "./Counter.vue";
export default {
  components: {
    Counter
  },
  name: 'Show',
  props: ['id','name','episodes_seen']
};
</script>

<style>
</style>
