<template>
  <div>
    <p>{{count}}</p>
    <button label v-on:click="count += 1">
      Increment
    </button>
    <button v-on:click="count -= 1">
      Decrement
    </button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      count: this.epsSeen
    }
  },
  props: {
    epsSeen: {
      type: Number,
      default: 0
    }
  }
  
};
</script>

<style>
</style>

