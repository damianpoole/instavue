<template>
    <div class="card">
        <Usertar :user="user"/>
        <img v-bind:src="require(`../assets/${imgUrl}`)"/>
    </div>
</template>

<script>
import Usertar from "@/components/Usertar.vue";

export default {
  name: "Card",
  props: {
    user: String,
    imgUrl: String
  },
  components: {
    Usertar
  }
};
</script>

<style scoped lang="stylus">
div.card {
    border: solid 1px #ccc;
    border-radius: 3px;
    width: 600px;
    min-height: 450px;
    display: block;
    margin: 5px auto;
}

img {
    max-width: 100%;
    max-height: 100%;
}
</style>
