<template>
  <div class="header-container">
    <div class="logo">
        <img alt="Vue logo" src="../assets/img/dc-logo.png">
    </div>
    <div class="menu">
        <ul v-for="(navMenuItem, index) in navMenuItems" :key="index">
            <li><a href="#" target="_blank" rel="noopener">{{navMenuItem}}</a></li>
            <!-- <li><a href="#" target="_blank" rel="noopener">CHARACTERS</a></li>
            <li><a href="#" target="_blank" rel="noopener">COMICS</a></li>
            <li><a href="#" target="_blank" rel="noopener">MOVIES</a></li>
            <li><a href="#" target="_blank" rel="noopener">TV</a></li>
            <li><a href="#" target="_blank" rel="noopener">GAMES</a></li>
            <li><a href="#" target="_blank" rel="noopener">COLLECTIBLES</a></li>
            <li><a href="#" target="_blank" rel="noopener">VIDEOS</a></li>
            <li><a href="#" target="_blank" rel="noopener">FANS</a></li>
            <li><a href="#" target="_blank" rel="noopener">NEWS</a></li>
            <li><a href="#" target="_blank" rel="noopener">SHOP</a></li> -->
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',

  data () {
    return {
    navMenuItems: ['CHARACTERS', 'COMICS', 
    'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEOS', 'FANS', 'NEWS', 'SHOP',]
    }
        

  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';

.header-container {
    @include flex-row-around;
      .logo {
      width: 40%;
        img {
        max-height: 60px;
        }
      }
      .menu {
      @include flex-row-around;
      width: 60%;
      padding-right: 10%;
        ul {
        list-style-type: none;
        padding: 0;
        margin: 1em 0 0 0;
          li {
            @include li-menu-horizontal;
            margin: 0 10px;
            height: 50px;
            &:hover {
              border-bottom: $colorBlue solid 2px;
            }
            a {
              color: #000;
              text-decoration: none;
              &:hover {
              color: $colorBlue;
              }
            }
          }
        }
      }
}



</style>