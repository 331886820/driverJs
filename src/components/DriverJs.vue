<template>
  <div>
    <div id="first" class="hello">
      <h1>{{ msg }}</h1>
    </div>
    <div id="second">
      <h1>driverJS</h1>
    </div>
    <div id="img1">
      <img src="@/assets/1.png" alt="">
    </div>
    <div id="img2">
      <img src="@/assets/2.png" alt="">
    </div>
    <div id="img3">
      <img src="@/assets/3.png" alt="">
    </div>
    <div id="img4">
      <img src="@/assets/4.png" alt="">
    </div>
    <div id="img5">
      <img src="@/assets/5.png" alt="">
    </div>
  </div>
</template>

<script>
import { driver } from "driver.js";
import "driver.js/dist/driver.css";

export default {
  name: "DriverJs",
  props: {
    msg: String,
  },
  created() {
    this.useDriver();
  },
  methods: {
    useDriver() {
      const driverObj = driver({
        showProgress: true,
        steps: [
          {
            element: "#first",
            popover: {
              title: "Animated Tour Example",
              description:
                "Here is the code example showing animated tour. Let's walk you through it.",
              side: "left",
              align: "start",
            },
          },
          {
            element: "#second",
            popover: {
              title: "Import the Library",
              description:
                "It works the same in vanilla JavaScript as well as frameworks.",
              side: "bottom",
              align: "start",
            },
          },
          {
            element: "#img1",
            popover: {
              title: "YG is the best",
              description:
                "https://juejin.cn/user/501800125607752/posts",
              side: "bottom",
              align: "start",
            },
          },
          {
            element: "#img2",
            popover: {
              title: "YG is the best",
              description:
                "https://juejin.cn/user/501800125607752/posts",
              side: "bottom",
              align: "start",
            },
          },
          {
            element: "#img3",
            popover: {
              title: "YG is the best",
              description:
                "https://juejin.cn/user/501800125607752/posts",
              side: "bottom",
              align: "start",
            },
          },
          {
            element: "#img4",
            popover: {
              title: "YG is the best",
              description:
                "https://juejin.cn/user/501800125607752/posts",
              side: "bottom",
              align: "start",
            },
          },
          {
            element: "#img5",
            popover: {
              title: "YG is the best",
              description:
                "https://juejin.cn/user/501800125607752/posts",
              side: "bottom",
              align: "start",
            },
          }
        ],
      });

      driverObj.drive();
    },
  },
};
</script>
<style scoped>
#first {
  background: #42b983;
}
#second {
  background: #737bea;
}
img {
  width:100%;
}
h3 {
  margin: 40px 0 0;
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
