<template>
  <div id="app">
      <main class="flexbox">


        <Board id="board-1">
          <Card id="card-1" draggable="true">
            <p>Card one</p>
          </Card>
        </Board>


        <Board id="board-2">
          <Card id="card-2" draggable="true">
            <p>Card two</p>
          </Card>
        </Board>
      </main>
  </div>
</template>

<script>
import Board from "./components/Board.vue";
import Card from "./components/Card.vue";

export default {
  name: 'App',
  components: {
    Board,
    Card

  }
}
</script>

<style>

*{
  margin:0;
  padding:0;
  box-sizing:border-box;

}

body{
  background-color: #F3F3F3;

}

.flexbox{
  display:flex;
justify-content: space-between;

  widht:100%;
  max-width: 760px;
  height: 100vh;
  overflow: hidden;



  padding: 15px;

}


.flexbox .board{
  display:flex;
  flex-direction: column;

  width: 100%;
  max-width: 300px;
  background-color: #313131;
padding: 15px;
}


.flexbox .board .card{
  padding:15px 25px;
  background-color: #f3f3f3;

  cursor:pointer;
  margin-bottom: 15px;
}
</style>
