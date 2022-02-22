<template>
<div class="full-footer-container">
    <ShopBanner
        v-for="(shopBannerItem,x) in shopBannerItems" 
        :key="x"
        :items="shopBannerItems"
     />
    
  <div class="footer-container">    
    <div class="footer-left">
        <div class="menu-col">
            <h6>DC COMICS</h6>
            <ul class="menu-col" v-for="(dcComicsItem, a) in dcComicsItems" :key="a">
                <li><a href="#" target="_blank" rel="noopener">{{dcComicsItem}}</a></li>
                <!--<li><a href="#" target="_blank" rel="noopener">Characters</a></li>
                <li><a href="#" target="_blank" rel="noopener">Comics</a></li>
                <li><a href="#" target="_blank" rel="noopener">Movies</a></li>
                <li><a href="#" target="_blank" rel="noopener">TV</a></li>
                <li><a href="#" target="_blank" rel="noopener">Games</a></li>
                <li><a href="#" target="_blank" rel="noopener">Videos</a></li>
                <li><a href="#" target="_blank" rel="noopener">News</a></li>-->
            </ul>
            <h6>SHOP</h6>
            <ul class="menu-col" v-for="(shopItem, b) in shopItems" :key="b">
                <li><a href="#" target="_blank" rel="noopener">{{shopItem}}</a></li>
                <!--<li><a href="#" target="_blank" rel="noopener">Shop DC</a></li>
                <li><a href="#" target="_blank" rel="noopener">Shop DC Collectibles</a></li>-->
            </ul>
        </div>
        <div class="menu-col">
            <h6>DC</h6>
            <ul class="menu-col" v-for="(dcItem, c) in dcItems" :key="c">
                <li><a href="#" target="_blank" rel="noopener">{{dcItem}}</a></li>
                <!--<li><a href="#" target="_blank" rel="noopener">Terms of Use</a></li>
                <li><a href="#" target="_blank" rel="noopener">Privacy Policy (new)</a></li>
                <li><a href="#" target="_blank" rel="noopener">Ad Choices</a></li>
                <li><a href="#" target="_blank" rel="noopener">Advertising</a></li>
                <li><a href="#" target="_blank" rel="noopener">Jobs</a></li>
                <li><a href="#" target="_blank" rel="noopener">Subscriptions</a></li>
                <li><a href="#" target="_blank" rel="noopener">Talent Workshops</a></li>
                <li><a href="#" target="_blank" rel="noopener">CPSC Certifications</a></li>
                <li><a href="#" target="_blank" rel="noopener">Ratings</a></li>
                <li><a href="#" target="_blank" rel="noopener">Shop Help</a></li>
                <li><a href="#" target="_blank" rel="noopener">Contact Us</a></li>-->
            </ul>
        </div>
        <div class="menu-col">
            <h6>SITES</h6>
            <ul class="menu-col" v-for="(sitesItem, d) in sitesItems" :key="d">
                <li><a href="#" target="_blank" rel="noopener">{{sitesItem}}</a></li>
                <!--<li><a href="#" target="_blank" rel="noopener">DC</a></li>
                <li><a href="#" target="_blank" rel="noopener">MAD Magazine</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Kids</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Universe</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Power Visa</a></li>-->
            </ul>
        </div>
    </div>
    <div class="footer-right">
        <img src="../assets/img/dc-logo-bg.png" alt="Big Logo">
    </div>

    <div class="footer-bottom-banner">
        <div class="footer-left">
            <button><a href="#" id="button">SIGN UP NOW</a></button>
        </div>
        <ul class="menu-row footer-right">
            <li><a href="#" target="_blank" rel="noopener" id="follow">FOLLOW US</a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/img/footer-facebook.png" alt="facebook"></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>            
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/img/footer-youtube.png" alt="youtube"></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/img/footer-periscope.png" alt="periscope"></a></li>
        </ul>
    </div>
  </div>
</div>
</template>

<script>

import ShopBanner from './partials/ShopBanner.vue'

export default {
    components: {ShopBanner},
    name: 'FooterComponent',

  data () {
      return {
          shopBannerItems: [
              {
                  text: 'DIGITAL COMICS',
                  src: '../../img/buy-comics-digital-comics.png',
              },
              {
                  text: 'DC MERCHANDISE',
                  src: '../../img/buy-comics-merchandise.png',
              },
              {
                  text: 'SUBSCRIPTION',
                  src: '../../img/buy-comics-subscriptions.png',
              },
              {
                  text: 'COMIC SHOP LOCATOR',
                  src: '../../img/buy-comics-shop-locator.png',
              },
              {
                  text: 'DC POWER AREA',
                  src: '../../img/buy-dc-power-visa.svg',
              },

          ],
          dcComicsItems: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News',
          ],
          shopItems: [
              'Shop DC',
              'Shop DC Collectibles',
          ],
          dcItems: [
              'Terms of Use',
              'Privacy Policy (new)',
              'Ad Choices',
              'Advertising',
              'Jobs',
              'Subscriptions',
              'Talent Workshops',
              'CPSC Certifications',
              'Ratings',
              'Shop Help',
              'Contact Us',
          ],
          sitesItems: [
              'DC',
              'MAD Magazine',
              'DC Kids',
              'DC Universe',
              'DC Power Visa',

          ],
          /*footerRightItems: [
              {
                  text: 'FOLLOW US',
                  img: '',
              },
              {
                  text: 'facebook',
                  img: 'footer-facebook.png',
              },
                            {
                  text: 'twitter',
                  img: 'footer-twitter.png',
              },
                            {
                  text: 'youtube',
                  img: 'footer-youtube.png',
              },
                            {
                  text: 'pinterest',
                  img: 'footer-pinterest.png',
              },
                            {
                  text: 'periscope',
                  img: 'footer-periscope.png',
              },
          ],*/
      }
  }

}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';

* {
    @include body-rules;
    text-align: left;
    color: #fff;
}

.full-footer-container {
    position: relative;
}

/* shop container

.shop-container {
    @include flex-row-around;
    background-color: $colorBlue;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;

    #shop-list {
    list-style-type: none;
    padding: 0;
    height: 100%;
    margin: auto;
    line-height: 70px;
    display: flex;
    align-self: center;

        li {
        @include li-menu-horizontal;
        margin: 0 10px;

            .shop-row {
            @include flex-row-center;
            color: #fff;
            text-decoration: none;
            

                .img-card {
                width: 40px;
                height: 40px;

                    img {
                    width: 100%;
                    height: 100%;
                    object-fit: contain;
                    padding-right: 10px;
                    }

                    h6 {
                    padding-left: 10px;
                    }


                }
            }
        }
    }
}
*/

/*main footer contents */

.footer-container {
    @include flex-row-around;
    background-image: url("../assets/img/footer-bg.jpg");
    height: 400px;


    .footer-left {
        display: flex;
        width: 40%;
        padding: 5% 0 5% 15%;


        .menu-col {
            @include flex-column;

                h6 {
                padding: 10px;
                margin-top: 10px;
                }
                ul {
                list-style-type: none;
                padding: 0;

                    li {
                    display: inline-block;
                    margin: 0 10px;
                    font-size: 11px;
                    vertical-align: center;
                    padding: 0;

                        a {
                        text-decoration: none;
                        color: $colorGrey;
                        &:hover {
                            color: $colorWhite;
                        }
                        }
                    }
                }
                
        }
    }
}


.footer-right {
    width: 60%;
    @include flex-row-center;

        img {
        max-height: 400px;
        padding-left: 5%;
        }
        a {
            text-decoration: none;
        }
}        


/*footer bottom banner */

.footer-bottom-banner {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 70px;
    background-color:#242424;
    display: flex;
    width: 100%;
}

.footer-bottom-banner img {
    max-height: 20px;
}

#follow {
    color: $colorBlue;
}

.footer-right li {
    @include li-menu-horizontal;
    margin: 0 5px;

}

button {
    align-self: center;
    padding: 10px;
    background-color: transparent;
    border: solid;
    border-color: #0c69f7;
    position: absolute;
    top: 15px;
    left: 15%;

    #button {
        text-decoration: none;
        color: $colorWhite;
    }
}



    




</style>