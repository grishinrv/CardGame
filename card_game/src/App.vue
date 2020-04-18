<template>
  <div id="app">
    <main class="flexbox">
      <Board id="board-1">
        <Card id="card-1" draggable="true"></Card>
        <Card id="card-2" draggable="true"></Card>
        <Card id="card-3" draggable="true"></Card>
      </Board>

      <Board id="board-2">
        <Card id="card-4" draggable="true"></Card>
      </Board>
    </main>
  </div>
</template>

<script>
import Board from './components/Board'
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    Board,
    Card
  }
}
</script>

<style>
body {
    background-color: grey;
}
.flexbox{
  display: flex;
  flex-direction: row;
  justify-content: space-between;

  width: 100%;
  max-width: 1920px;
  height: 500px;

  overflow: hidden;

  margin: 0 auto;
  padding: 15px;
}

.flexbox .board{
  display: flex;

  width: 100%;
  max-width: 500px;
  height: 480px;

  background-color: bisque;
  border-color: black;
  border-width: 1px;
  border-style: solid;

  padding: 15px;
}
</style>
