<script>
// import { ref } from "vue";
// const msg1 = ref("Hello from MyComponent.vue");
// const msg5 = ref("eeeHello from MyComponent.vue");

// const BASE = "https://admin.qm-vip.com/hk_admin";
export default {
  data() {
    return {
      msg5: "dd",
    };
  },
  props: {
    msg1: String,
    msg2: String,
  },
  // computed: {
  //   fullUrl() {
  //     return (this.isAssetsHost == null ? this.$cfg.assetshost : "") + this.src;
  //   },
  // },
};
</script>
<template>
  <p class="msg1">{{ msg1 }}</p>
  <p class="msg2">{{ msg2 }}</p>
  <!-- <p class="msg5">{{ msg5 }}</p> -->
</template>

<style>
.msg1 {
  color: rgb(182, 16, 30);
  font-weight: bold; /*字体*/
}
.msg2 {
  color: rgb(10, 63, 28);
  font-weight: bold; /*字体*/
}
</style>
