<template>
  <div>
    X : <input type="text" v-model.number="state.x" /><br />
    <div>결과 : {{ result }}</div>
  </div>
</template>

<script>
import { watch, ref } from 'vue'

export default {
  name: 'Calc5',
  setup() {
    const x = ref(0)
    const result = ref(0)
    watch(x, (current, old) => {
      console.log(`${old} ==> ${current}`)
      result.value = current * 2
    })
    return { x, result }
  },
}
</script>
