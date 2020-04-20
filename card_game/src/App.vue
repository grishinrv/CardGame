<template>
  <div id="app">
    <main class="flexbox">
      <Board id="board-1">
        <Card id="card-1" draggable="true" avatar="https://cdnb.artstation.com/p/assets/images/images/018/433/397/large/anton-evsyukov-blood-elf.jpg?1559343941"></Card>
        <Card id="card-2" draggable="true" avatar="https://i.pinimg.com/originals/33/d5/6f/33d56f85496956d2f3e1bb1bb91616b2.jpg"></Card>
        <Card id="card-3" draggable="true" avatar="https://cdnb.artstation.com/p/assets/images/images/019/518/927/large/paul-mafayon-anka-the-buried-final.jpg?1563863853"></Card>
      </Board>

      <Board id="board-2">
        <Card id="card-4" draggable="true" avatar="https://natpagle.ru/wp-content/uploads/2019/06/Madame-Lazul-art.jpg"></Card>
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

  flex-wrap: wrap;
  justify-content: space-around;

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
