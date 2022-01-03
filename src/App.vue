<template>
  <div id="app">
    <div class="row w-100" d-flex justify-content-center align-items-center>
      <div class="card">
        <Header/>
        <Todo/>
        <Todolist/>
        <Footer/>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Todo from './components/Todo.vue'
import Todolist from './components/Todolist.vue'
export default {
  name:'App',
  components:{
    Todo,
    Todolist,
    Header,
    Footer,
  }
  
}
</script>

<style >
* {
  box-sizing: border-box;
  position: relative;
  margin: 0;
  padding: 0;
}
#app {
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: orange;
}
.card{
  min-height: 500px;
  width: 50%;
}
</style>