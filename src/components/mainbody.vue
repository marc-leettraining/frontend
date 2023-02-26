<template>
  <h1>{{ msg }}</h1>
  <div id="container">
    <div class="vision">
      <h3>
        Our mission is to empower professionals with the knowledge and skills
        they need to excel in their current roles or reach their career goals.
        We offer customized training programs that are tailored to the specific
        needs of our clients, whether they are looking to move up the ladder or
        get started in a new career vertical.
      </h3>
    </div>
    <div class="door">
      <img src="../assets/door.png" />
    </div>
    <div class="how">
      <h2>How it works:</h2>
      <h3>
        Our training programs keep up with the latest technologies and best
        practices, and we use a flexible approach that allows us to adapt to the
        unique needs of our clients. We provide on-demand training when needed,
        so professionals can learn at their own pace and on their own schedule.
      </h3>
    </div>
    <div class="goal">
      <h2>Our goal:</h2>
      <h3>
        By partnering with us, professionals will have the tools they need to
        succeed in their roles or take the next step in their careers, all while
        staying competitive in their rapidly evolving industry.
      </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 2fr 2fr 2fr 2fr;
  grid-template-areas:
    "vision vision vision"
    "door how how"
    "door goal goal";
  grid-gap: 3px;
  margin: auto;
  width: 90%;
}

.vision {
  grid-area: vision;
  border: 3px solid #307ED0;
}

.door {
  grid-area: door;
}

.door img {
  width: 100%;
  height: 100%;
  max-width: MaxSize;
  max-height: MaxSize;
  overflow: hidden;
}

.how {
  grid-area: how;
  text-align: left;
}
.goal {
  grid-area: goal;
  text-align: left;
}

h2 {
  text-align: lext;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
