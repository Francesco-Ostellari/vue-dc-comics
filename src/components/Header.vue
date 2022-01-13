<template>
  <header>
    <div class="header-container flex">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li> <a href="#">characters</a> </li>
        <li> <a href="#">comics</a> </li>
        <li> <a href="#">movies</a> </li>
        <li> <a href="#">tv</a> </li>
        <li> <a href="#">games</a></li>
        <li> <a href="#">collectibles</a> </li>
        <li> <a href="#">videos</a> </li>
        <li> <a href="#">fans</a> </li>
        <li> <a href="#">news</a> </li>
        <li> <a href="#">shop</a> </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() { 
    return {
      
    }
  }, 
  created () {

  },
  methods: {
    
  }
}
</script>

<style lang="scss" scoped>
  header {
    background-color: white;
    height: 100px;
    width: 100%;
  }

  .flex {
    display: flex;
  }

  .header-container {
    width: 70%;
    height: 100%;
    margin: 0 auto;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
  }

  .header-container img {
    height: 100%;
  }
  
  .header-container ul {
    text-decoration: none;
  }

  .header-container ul li {
    text-decoration: none;
    display: inline-block;
    margin-right: 20px;
    text-transform: uppercase;
  }

  .header-container ul li a {
    text-decoration: none;
    color: #1C1C1C;
    font-weight: 800;
  }
</style>