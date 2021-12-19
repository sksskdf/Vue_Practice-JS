<template>

  <div class="menu">
    <a v-for="(a) in menu" :key="a">{{a}}</a>
  </div>

  <div>
    <h4>{{products[0]}} 원룸</h4>
    <p>10 만원</p>
    <button @click="increase(0)">허위매물신고</button> <span>신고수 : {{신고수[0]}}</span>
  </div>
  <div>
    <h4>{{products[1]}} 원룸</h4>
    <p>10 만원</p>
    <button @click="increase(1)">허위매물신고</button> <span>신고수 : {{신고수[1]}}</span>
  </div>
  <div>
    <h4>{{products[2]}} 원룸</h4>
    <p>10 만원</p>
    <button @click="increase(2)">허위매물신고</button> <span>신고수 : {{신고수[2]}}</span>
  </div>


  
</template>

<script>


export default {
  name: 'App',
  data(){
    return {
      신고수 : [0,0,0],
      menu : ['Home','Products','About'],
      products : ['역삼동원룸','천호동원룸','마포구원룸'],
    }
  },
  methods : {
    increase(i){
      this.신고수[i] ++;
    }
  },
  components: {

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
.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}

.menu a {
  color: white;
  padding:10px;

}
</style>
