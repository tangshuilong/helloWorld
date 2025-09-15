<script>
export default {
  data() {
    return {};
  },

  props: {
    msg3: String,
    msg4: String,
    msg5: String,
    msg6: String,
    msg7: String,
  },
};
</script>

<template>
  <p class="msg3">{{ msg3 }}</p>
  <p class="msg4">{{ msg4 }}</p>
  <p class="msg5">{{ msg5 }}</p>
  <p class="msg6">{{ msg6 }}</p>
  <p class="msg7">{{ msg7 }}</p>
</template>

<style>
.msg3 {
  color: rgb(19, 94, 31);
  font-weight: bold; /*字体*/
}
.msg4 {
  color: rgb(12, 202, 75);
  font-weight: bold; /*字体*/
}
.msg5 {
  color: rgb(226, 7, 7);
  font-weight: bold; /*字体*/
}
.msg6 {
  color: #087bda;
  font-weight: bold; /*字体*/
}
.msg7 {
  color: #6eda08;
  font-weight: bold; /*字体*/
}
</style>
