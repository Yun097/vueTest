<template>
  <div class="hello" :class="type">
    <div class="img" v-for="item in 3" :key="item">
      <img alt="Vue logo" :src="require(`@/assets/logo.png`)" >
    </div>
    <div>
      <p>{{ title }}</p>
      <p>{{ msg }}</p>
      <button>+</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: String,
    msg: String,
    type: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hello{
  width: 100%;
  display: inline-flex;
  margin: 1rem;
}
.img{
  width: 5rem;
  height: 5rem;
  background-color: #fff;
  margin: 100px;
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
