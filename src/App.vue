<template>
<header>
  <h1>Asafa</h1>
  <form action="" class="search" @submit="searchTitle">
    <input type="search" class="search-bar" placeholder="search a title" v-model="title">
  <button class="submit-btn">search</button>
  </form>

</header>
<main>
  <div class="menu-and-contains">
  <div class="menu-bars">  
    <p>Home</p>
    <p>Search</p>
    <p>Singers</p>
    <p>Title sing</p>
    <p>Settings</p>
    <p>About</p>
  </div>
  <div class="home">
<h2>Welcome to Asafa</h2>
  </div>
    </div>
</main>
</template>

<script setup>
import { ref } from 'vue';

const title = ref('')

</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html,body{
  height: 100%;
  width: 100%;
}
header{
  color: white;
  display: flex;
  justify-content: space-around;
  background-color: rgb(0, 31, 46);
  align-items: center;
  text-align: center;
  padding: 2vh;
}
main{
  height: calc(100vh - 70px);
  color: white;
  display: flex;
  background: 
    linear-gradient(rgba(0, 0, 0, 0.95)),
    url('@/assets/images/backgrounds/song-7058726_1280.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
  }
.menu-bars{
  background-color: rgb(0, 31, 46);
  color: white;
  display: flex;
  flex-direction: column;
  font-size: x-large;
  align-items: center;
  height: 100%;
  width: 10vw;
  min-width: 150px;
  padding-top: 2rem;
  justify-content: space-evenly;
}
.menu-and-contains{
  display: flex;
  width: 100%;
  
}
.menu-bars p{  
  text-align: center;
  width: 100%;
  padding-block: 3rem;
}
.menu-bars p:hover{
  opacity: 80%;
  background-color: rgb(192, 131, 0);
  text-align: center;
  width: 100%;
}
.search{
  display: flex;
}
.search-bar{
 padding-block: 1vh;
 width: 20vw;
}
.submit-btn{
  padding-inline: 1rem;
  background-color: white;
}
.home{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  font-size: xx-large;
}
</style>