<script>
export default {
  data() {
    return {};
  },
  props: {
    msg8: String,
  },
};
</script>

<template>
  <p class="msg8">{{ msg8 }}</p>
</template>

<style>
.msg8 {
  color: red;
  font-weight: bold; /*字体*/
}
</style>
