<template>
  <div class="home">
    <Card 
      imgUrl="dpool.jpg" 
      user="Damian Poole"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from "@/components/Card.vue";

export default {
  name: "home",
  components: {
    Card
  }
};
</script>

<style lang="stylus" scoped>
.home {
  background: #f3f3f3;
  text-align: left;
  padding: 15px 0;
}
</style>
