<script>
// import { ref } from "vue";
// const msg3 = ref("Hello from MyComponent.vue------");
// const msg4 = ref("Hello from MyComponent.vue------");
export default {
  data() {
    return {};
  },
  props: {
    msg3: String,
    msg4: String,
  },
};
</script>

<template>
  <p class="msg3">{{ msg3 }}</p>
  <p class="msg4">{{ msg4 }}</p>
</template>

<style>
.msg3 {
  color: rgb(14, 27, 209);
  font-weight: bold; /*字体*/
}
.msg4 {
  color: rgb(12, 202, 75);
  font-weight: bold; /*字体*/
}
</style>
