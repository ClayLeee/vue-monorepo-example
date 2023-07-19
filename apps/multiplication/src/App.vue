<template>
  <div id="app" style="
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 60px;
    color: red;"
  >
    <div>This is multiplication project</div>
    <div>a = {{ a }}, b= {{ b }}</div>
    <div>a * b = {{ multiplication(a, b) }}</div>
    <br>
    <br>
    <div>Multiplication with addition</div>
    <div>a = {{ a }}, b = {{ b }}, c = {{ c }}</div>
    <div>(a * b) + c = {{ addMultiply(a, b, c) }}</div>
  </div>
</template>

<script>
import { addition, multiplication } from '@shared/utils/calculation'

export default {
  name: 'App',
  data() {
    return {
      a: 3,
      b: 4,
      c: 5
    }
  },
  computed: {
    multiplication() {
      return (a, b) => multiplication(a, b)
    },
    addMultiply() {
      return (a, b, c) => addition(multiplication(a, b), c)
    }
  }
}
</script>
