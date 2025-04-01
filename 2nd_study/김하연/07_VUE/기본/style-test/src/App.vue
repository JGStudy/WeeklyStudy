<template>
  <div :class="$style.child">
    <h2>Child3</h2>
    <!-- <Child1 />
    <Child2 />
    <Child3 /> -->
  </div>
</template>
<script>
// import Child1 from './components/Child1.vue';
// import Child2 from './components/Child2.vue';
// import Child3 from './components/Child3.vue';
export default {
  // name: 'App',
  // components: { Child1, Child2, Child3 },
  name: 'Child3',
  created() {
    console.log(this.$style.child);
  },
};
</script>
<style module>
.child {
  background-color: orange;
  border: solid 1px black;
  margin: 1.5rem;
  padding: 1rem;
}
</style>
