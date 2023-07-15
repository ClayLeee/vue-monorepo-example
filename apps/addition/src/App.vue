<template>
  <div id="app">
    {{ addition(a, b) }}
  </div>
</template>

<script>
import { addition } from '@shared/ui'

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
