<template>
  <div>
    <input type="text" v-model="num1" />
    <input type="text" v-model="num2" />
    <button @click="calculateSum">Calculate</button>
    <p>Sum: {{ sum }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num1: 0,
      num2: 0,
      sum: 0,
    };
  },
  methods: {
    calculateSum() {
      this.sum = Number(this.num1) + Number(this.num2);
    },
  },
};
</script>
