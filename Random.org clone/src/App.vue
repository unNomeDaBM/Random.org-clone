<template>
  <body>
    <div class="content">
      <NavLinks/>
      <TitleComponent/>
      <MainRandom/>
      <ThingsBelow/>
      <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
    </div>
  </body>
</template>

<script>
import MainRandom from './components/Sigleton Components/MainRandom.vue';
import NavLinks from './components/Sigleton Components/NavLinks.vue';
import TitleComponent from './components/Sigleton Components/TitleComponent.vue';

  export default{
    data(){
      return{

      }
    },
    components:{NavLinks, TitleComponent, MainRandom}
  }
</script>

<style>
  body{
    display: grid;
    justify-items: center;
    font-family: sans-serif;
  }

  a{
    text-decoration: none;
  }

  .content{
    width: 800px;
    background-color: #c3c3c3; /* To remove later */   
  }
</style>