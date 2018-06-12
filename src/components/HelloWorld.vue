<template>
  <div class="hello">
    <h3>{{ msg }}</h3>
    <section id="section07" class="demo">
      <a href="#generator"><span></span><span></span><span></span></a>
    </section>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  font-size: 1.6rem;
  font-style: italic;
  line-height: 1.7rem;
  color: #7f38f5;
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

/*section scrolldown*/
section {
  position: relative;
  width: 100%;
  height: 100%;
}
section::after {
  position: absolute;
  bottom: 0;
  left: 0;
  content: "";
  width: 100%;
  height: 80%;
  background: -webkit-linear-gradient(
    top,
    rgba(0, 0, 0, 0) 0,
    rgba(0, 0, 0, 0.8) 80%,
    rgba(0, 0, 0, 0.8) 100%
  );
  background: linear-gradient(
    to bottom,
    rgba(0, 0, 0, 0) 0,
    rgba(0, 0, 0, 0.8) 80%,
    rgba(0, 0, 0, 0.8) 100%
  );
}

.demo a {
  position: absolute;
  top: 11rem;
  left: 51.7%;
  transform: translate(-50%, -50%);
  z-index: 2;
  display: inline-block;
  color: rgb(228, 49, 49);
  font: normal 400 12px/1 "Josefin Sans", sans-serif;
  letter-spacing: 0.1em;
  text-decoration: none;
  transition: opacity 0.3s;
}
.demo a:hover {
  opacity: 0.5;
}

#section07 a span {
  position: absolute;
  top: 0;
  left: 50%;
  width: 1.1rem;
  height: 1.1rem;
  margin-left: -12px;
  border-left: 1px solid rgba(73, 152, 226, 0.719);
  border-bottom: 1px solid rgba(223, 68, 68, 0.719);
  -webkit-transform: rotate(-45deg);
  transform: rotate(-45deg);
  -webkit-animation: sdb07 2s infinite;
  animation: sdb07 2s infinite;
  opacity: 0;
  box-sizing: border-box;
}
#section07 a span:nth-of-type(1) {
  -webkit-animation-delay: 0s;
  animation-delay: 0s;
}
#section07 a span:nth-of-type(2) {
  top: 16px;
  -webkit-animation-delay: 0.15s;
  animation-delay: 0.15s;
}
#section07 a span:nth-of-type(3) {
  top: 32px;
  -webkit-animation-delay: 0.3s;
  animation-delay: 0.3s;
}
@-webkit-keyframes sdb07 {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@keyframes sdb07 {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
</style>
