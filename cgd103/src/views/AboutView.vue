<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Button type="primary">Primary</Button>
    <hr>
    <div>
      <Carousel v-model="value" loop>
        <CarouselItem v-for="item in 5" :key="item">
          <div class="demo-carousel">123
            <!-- <img :src="require(`@/assets/logo.png`)"> -->
          </div>
        </CarouselItem>
      </Carousel>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

