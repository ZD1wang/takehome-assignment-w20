<template>
  <div class="counter">
    <p>I'm a Counter!</p>
    <div>
      <!-- Part 3 -->
      <button v-on:click="add1()"> Add 1 </button>
      <button v-on:click="substract1()"> Substract 1 </button>
      <p> The value of the current count: {{counter}}. </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    counter: Number
  },
  data() {
    return {
      count: (this.count)
    };
  },
  methods: {
    add1: function() {
      this.counter += 1;
    },
    substract1: function() {
      this.counter -= 1;
    }
  }
};
</script>

<style scoped>
.counter {
  display: block;
}
</style>

