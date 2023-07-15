<template>
  <div id="app">
    {{ multiplication(a, b) }}
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
