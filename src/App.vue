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
  height: 240px;
  width: 240px;
  border-radius: 50%;
  background-color: #f4cd2a;
  border: 5px solid #eda323;
  font-size: 140px;
  color: #eda323;
}

.button:active {
  margin: 3px;
  height: 234px;
  width: 234px;
  font-size: 136px;
  transition: 2ms;
}
</style>
