<template>
    <div class="usertar">
        <v-avatar
            :tile="tile"
            :size="32">
            <img src="../assets/myAvatar.png"/>
        </v-avatar>
        <span>
            {{ user }}
        </span>
    </div>
</template>

<script>
export default {
  name: "Usertar",
  props: {
    user: String
  }
};
</script>

<style lang="stylus" scoped>
.usertar {
    font-weight: bold;
    margin: 15px;
}

span {
    margin-left: 10px;
    display: inline-block;
}
</style>
