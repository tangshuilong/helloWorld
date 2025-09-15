<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  <h1>{{ tips1 }}</h1>
  <h2>{{ number }}</h2>
  <h3>{{ nIndex }}</h3>
  <h4>{{ tips2 }}</h4>
  <h5>{{ tips4 }}</h5>
  <button @click="addNumber">Count---2 is: {{ number }}</button>
  <button @click="addIndex">vv: {{ nIndex }}</button>
  <MyComponent msg1="kkkfff---1111qqccvv" />
  <MyComponent msg2="kkkfff---2222qqccvv" />
  <MyComponentTips {{ msg3="111111--222222--333333--444444--555555" }} />
  <HelpComponent
    msg3="HelpComponent--msg3333"
    msg4="HelpComponent--msg4444"
    msg5="HelpComponent--msg5555"
    msg6="HelpComponent--msg6666"
    msg7="HelpComponent--msg7777"
  />
  <ActivityComponent msg8="ActivityComponent--msg8888" />
</template>

<script>
import { ref } from "vue";
// import HelloWorld from "./components/HelloWorld.vue";
import MyComponent from "./components/MyComponent.vue";
import MyComponentTips from "./components/MyComponentTips.vue";
import HelpComponent from "./components/HelpComponent.vue";
import ActivityComponent from "./components/ActivityComponent.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    MyComponent,
    MyComponentTips,
    HelpComponent,
    ActivityComponent,
  },

  setup() {
    const nIndex = ref(1);

    function addIndex() {
      nIndex.value += 1;
    }
    return { nIndex, addIndex };
  },

  data() {
    return {
      tips1: "Welcome to Your Vue.js App--tips1",
      tips2: "Welcome to Your Vue.js App--tips2",
      tips3: "Welcome to Your Vue.js App--tips3",
      tips4: "Welcome to Your Vue.js App--tips4",
      count: 0,
      number: 0,
    };
  },

  methods: {
    addNumber() {
      this.number += 1;
    },
    subNuber() {
      this.number -= 1;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #312c50;
  margin-top: 0px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
}
</style>
