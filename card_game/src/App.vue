<template>
  <div id="app">
    <div id="gameContainer">
      <!-- 
          Прочитайте статью:
          https://ru.vuejs.org/v2/guide/components-props.html
      -->
      <!-- передать каждому экземпляру компонента Card разные данные-->
      <Card />
      <Card />
    </div>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'App',
  data(){ //функция data() - js метод, который возвращает массив
    return { // функция return
      cardData: [
//заполнить массив данными для последующей передачи в экземпляры Card
      ]
    }
  },
  components: {
    Card
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#gameContainer{
  display: flex;
  justify-content: space-around;
}
</style>
