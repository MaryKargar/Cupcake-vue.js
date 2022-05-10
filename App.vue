<template>
  <div>
    <card-componnent :cakes='cakes'></card-componnent>
  </div>
</template>

<script>
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css'
import CardComponnent from './components/CardComponnnent.vue'
export default {
  components:{
    CardComponnent
  },
  data(){
    return{
      cakes:[
        {title:'Chocolate CupCake', ingredients:'eggs, milk, oil, and vanilla', recipe:'Add the eggs, milk, oil, and vanilla. Mix on medium speed for about two minutes. Stir in boiling water. Dont worry if the batter seems a little thin, as reviewers say thats perfectly normal. ', img:'../assets/1.jpg' },
        {title:'vanilla CupCake', ingredients:'eggs, milk, oil, and vanilla', recipe:'Add the eggs, milk, oil, and vanilla. Mix on medium speed for about two minutes. Stir in boiling water. Dont worry if the batter seems a little thin, as reviewers say thats perfectly normal. ',img:'../assets/ch.jfif' },
        {title:'orange CupCake', ingredients:'eggs, milk, oil, and vanilla', recipe:'Add the eggs, milk, oil, and vanilla. Mix on medium speed for about two minutes. Stir in boiling water. Dont worry if the batter seems a little thin, as reviewers say thats perfectly normal. ',img:'../assets/ch.jfif' },
        {title:'strawberry  CupCake', ingredients:'eggs, milk, oil, and vanilla', recipe:'Add the eggs, milk, oil, and vanilla. Mix on medium speed for about two minutes. Stir in boiling water. Dont worry if the batter seems a little thin, as reviewers say thats perfectly normal. ',img:'../assets/ch.jfif' },
      ]
    }
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
  align-items : center;
  justify-content: center;
}

nav {
  padding: 30px;
  align-items : center;
  justify-content: center;
  
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  align-items : center;
  justify-content: center;
  
}

nav a.router-link-exact-active {
  color: #42b983;
  align-items : center;
  justify-content: center;
  
}
</style>
