<template>
  <TitleBar />
  <div id="bg-img">
    <Mainbody
      msg="Mark your calendars: Q1 2024 brings the latest advancements in training programs!"
    />
  </div>
</template>

<script>
import Mainbodyvue from "./components/mainbody.vue";
import TitleBarVue from "./components/TitleBar.vue";
export default {
  name: "App",
  components: {
    Mainbody: Mainbodyvue,
    TitleBar: TitleBarVue,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  --margin-top: 60px;
  background: #99D2F0;
}

/*#container {
  opacity: 0.2;
  position: absolute;
  --z-index: -1;
  width: 100%;
  height: 100%;
  object-fit: cover;
  overflow: hidden;
}*/

#bg-img {
  width: 100vw;
  height: 100vw;
  overflow: hidden;
  border-style: solid;
  border-width: 2px;
  background-repeat: repeat;
  background-image: url("./assets/logo.png");
}
</style>
