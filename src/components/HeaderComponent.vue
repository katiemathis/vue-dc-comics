<template>
  <div class="header-container">
    <div class="logo">
        <img alt="Vue logo" src="../assets/dc-logo.png">
    </div>
    <div class="menu">
        <ul>
            <li><a href="#" target="_blank" rel="noopener">CHARACTERS</a></li>
            <li><a href="#" target="_blank" rel="noopener">COMICS</a></li>
            <li><a href="#" target="_blank" rel="noopener">MOVIES</a></li>
            <li><a href="#" target="_blank" rel="noopener">TV</a></li>
            <li><a href="#" target="_blank" rel="noopener">GAMES</a></li>
            <li><a href="#" target="_blank" rel="noopener">COLLECTIBLES</a></li>
            <li><a href="#" target="_blank" rel="noopener">VIDEOS</a></li>
            <li><a href="#" target="_blank" rel="noopener">FANS</a></li>
            <li><a href="#" target="_blank" rel="noopener">NEWS</a></li>
            <li><a href="#" target="_blank" rel="noopener">SHOP</a></li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.header-container {
    display: flex;
    justify-content: space-around;
}

.logo {
    width: 40%;
    
}

img {
    max-height: 60px;
}

.menu {
    width: 60%;
    padding-right: 10%;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
  font-size: 11px;
  font-weight: 600;
  vertical-align: center;
}
a {
  color: #000;
  text-decoration: none;
}
</style>