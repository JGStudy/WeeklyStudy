<template>
  <div>
    x : <input type="text" v-model.number="x" />
    <br />
    결과 : {{ result }}
  </div>
</template>

<script>
import { ref, computed } from 'vue';

export default {
  name: 'Calc5',
  setup() {
    const x = ref(0);
    const result = computed(() => x.value * 2);

    return { x, result };
  },
};
</script>