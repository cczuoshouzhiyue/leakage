<template>
  <div id="app">
   <header>
     <router-link to="/">
       菜单1
     </router-link>
     <router-link to="/menu">
       菜单2
     </router-link>
   </header>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
header {
  margin-bottom: 50px;
  background: #eee;
  color: #fff;
  height: 60px;
}
body{
  margin: 0;
  padding: 0;
}
</style>
