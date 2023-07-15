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
  </div>
</template>

<script>
import { multiplication } from '@shared/utils/calculation'

export default {
  name: 'App',
  data() {
    return {
      a: 3,
      b: 4
    }
  },
  computed: {
    multiplication() {
      return (a, b) => multiplication(a, b)
    }
  }
}
</script>
