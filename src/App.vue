<template>
  <div class="wrapper">
    <h2>Clicker MiniApp Telegram</h2>
    <h3>Score: {{score}}</h3>
    <input class="button" type="button" value="$" @click="updateScore">
  </div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    score: 0
  }),
  methods: {
    updateScore() {
      this.score = this.score + 1
    }
  }
}
</script>

<style scoped lang="css">
.button {
  height: 150px;
  width: 150px;
  border-radius: 50%;
  background-color: #f4cd2a;
  border: 5px solid #eda323;
  font-size: 80px;
  color: #eda323;
}

.button:active {
  margin: 2px;
  height: 146px;
  width: 146px;
  font-size: 76px;
  transition: 2ms;
}
</style>
