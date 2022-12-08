<template>
  <div class="hello">
    <div class="img">
      <img src="" alt="">
    </div>
    <div>
      <p>{{ title }}</p>
      <p>{{ msg }}</p>
      <button>太快啦</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: String,
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hello{
  width: 100%;
  display: inline-flex;
}
.img{
  width: 5rem;
  height: 5rem;
  background-color: #fff;
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
