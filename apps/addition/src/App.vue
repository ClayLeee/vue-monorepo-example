<template>
  <div id="app" style="
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 60px;
    color: red;"
  >
    <div>This is addition project</div>
    <div>a = {{ a }}, b = {{ b }}</div>
    <div>a + b = {{ addition(a, b) }}</div>
  </div>
</template>

<script>
import { addition } from '@shared/utils/calculation'

export default {
  name: 'App',
  data() {
    return {
      a: 1,
      b: 2
    }
  },
  computed: {
    addition() {
      return (a, b) => addition(a, b)
    }
  }
}
</script>
