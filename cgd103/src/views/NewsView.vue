<template>
    <div class="news">
      <img alt="Vue logo" :src="require(`@/assets/logo.png`)">
      <button 
        v-for="i in colors" 
        :key="i"
        :class="{active: active === i}"
        @click="changeColor(i)"
      >{{i}}</button>
      {{active}}
    </div>
</template>
  
<script>
  import { Colors } from '@/assets/config/setting.js'
  export default {
    data(){
      return{
        colors: Colors,
        activeColor:''
      }
    },
    methods: {
        changeColor(color){
          console.log(color);
          this.activeColor = color
        },
        getProduct(){
          fetch('https://fakestoreapi.com/products/categories')
          .then(res=>res.json())
          .then(json=>console.log(json))
        }
    },
    created(){
      this.getProduct()
    },
    mounted(){},
  }
</script>

<style lang="scss">
.news{
    text-align: center;
    padding: 4rem;
    background: #fff;
}

.button{
  color: #fff;
  padding: 1.0rem 1rem;
  &:active{
  }
}
</style>
