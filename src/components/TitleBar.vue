<template>
  <div id="parent">
    <div id="burger">
      <div class="top-and-bottom-bar"></div>
      <div id="middle-bar"></div>
      <div class="top-and-bottom-bar"></div>
    </div>
    <div id="title">
      <img src="../assets/Untitled-1.png" id="title-img" />
    </div>
    <div id="logo">
      <img src="../assets/enhance-logo.jpg" id="logo-img" />
    </div>
  </div>
</template>

<script>
export default {
  name: "TitleBar",
};
</script>

<style scoped>
#parent {
  display: inline-flex;
  background: #E08C60;
  width: 100%;
  height: 120px;
  --border-width: 5px;
  --border-style: solid;
}

#burger {
  --border-style: solid;
  --border-width: 2px;
  width: 15%;
  display: block;
}

.top-and-bottom-bar {
  width: 60px;
  height: 10px;
  background-color: #99D2F0;
  margin-top: 20px;
  margin-right: 0px;
  margin-left: auto;
  margin-right: 0px;
}

#middle-bar {
  margin-top: 20px;
  width: 90px;
  height: 10px;
  background-color: #99D2F0;
  margin-left: auto;
  margin-right: 0px;
}

#title {
  --position: relative;
  --border-style: solid;
  --border-width: 2px;
  width: 70%;
}

#logo {
  --border-style: solid;
  --border-width: 2px;
  width: 15%;
}

li {
  display: inline;
  padding: 12px;
}

#title-img {
  max-width: 100%;
  --max-height: auto;
  --border-style: solid;
  --border-width: 2px;
  border-color: green;
  --height: auto;
  --display: block;
  --position: absolute;
  --margin-left: auto;
  --margin-right: auto;
}

#logo-img {
  width: 120px;
  height: 120px;
  --max-height: auto;
  --border-style: solid;
  --border-width: 2px;
  border-color: green;
  --height: auto;
  --display: block;
  --position: absolute;
  --margin-left: auto;
  --margin-right: auto;
}
</style>