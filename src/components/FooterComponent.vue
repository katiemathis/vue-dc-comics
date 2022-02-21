<template>
<div class="full-footer-container">
    <div class="shop-container">
        <ul id="shop-list">
            <li>
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img src="../assets/buy-comics-digital-comics.png">
                    </div>
                    <h6>DIGITAL COMICS</h6>
                </a>

            </li>
            <li>
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img src="../assets/buy-comics-merchandise.png">
                    </div>
                    <h6>DC MERCHANDISE</h6>
                </a>
            </li>
            <li>
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img src="../assets/buy-comics-subscriptions.png">
                    </div>
                    <h6>SUBSCRIPTIONS</h6>
                </a>
            </li>
            <li>
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img src="../assets/buy-comics-shop-locator.png">
                    </div>
                    <h6>COMIC SHOP LOCATOR</h6>
                </a>
            </li>
            <li>
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img src="../assets/buy-dc-power-visa.svg">
                    </div>
                    <h6>DC POWER VISA</h6>
                </a>
            </li>
        </ul>
  </div>
  <div class="footer-container">    
    <div class="footer-left">
        <div class="menu-col">
            <h6>DC COMICS</h6>
            <ul class="menu-col">
                <li><a href="#" target="_blank" rel="noopener">Characters</a></li>
                <li><a href="#" target="_blank" rel="noopener">Comics</a></li>
                <li><a href="#" target="_blank" rel="noopener">Movies</a></li>
                <li><a href="#" target="_blank" rel="noopener">TV</a></li>
                <li><a href="#" target="_blank" rel="noopener">Games</a></li>
                <li><a href="#" target="_blank" rel="noopener">Videos</a></li>
                <li><a href="#" target="_blank" rel="noopener">News</a></li>
            </ul>
            <h6>SHOP</h6>
            <ul class="menu-col">
                <li><a href="#" target="_blank" rel="noopener">Shop DC</a></li>
                <li><a href="#" target="_blank" rel="noopener">Shop DC Collectibles</a></li>
            </ul>
        </div>
        <div class="menu-col">
            <h6>DC</h6>
            <ul class="menu-col">
                <li><a href="#" target="_blank" rel="noopener">Terms of Use</a></li>
                <li><a href="#" target="_blank" rel="noopener">Privacy Policy (new)</a></li>
                <li><a href="#" target="_blank" rel="noopener">Ad Choices</a></li>
                <li><a href="#" target="_blank" rel="noopener">Advertising</a></li>
                <li><a href="#" target="_blank" rel="noopener">Jobs</a></li>
                <li><a href="#" target="_blank" rel="noopener">Subscriptions</a></li>
                <li><a href="#" target="_blank" rel="noopener">Talent Workshops</a></li>
                <li><a href="#" target="_blank" rel="noopener">CPSC Certifications</a></li>
                <li><a href="#" target="_blank" rel="noopener">Ratings</a></li>
                <li><a href="#" target="_blank" rel="noopener">Shop Help</a></li>
                <li><a href="#" target="_blank" rel="noopener">Contact Us</a></li>
            </ul>
        </div>
        <div class="menu-col">
            <h6>SITES</h6>
            <ul class="menu-col">
                <li><a href="#" target="_blank" rel="noopener">DC</a></li>
                <li><a href="#" target="_blank" rel="noopener">MAD Magazine</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Kids</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Universe</a></li>
                <li><a href="#" target="_blank" rel="noopener">DC Power Visa</a></li>
            </ul>
        </div>
    </div>
    <div class="footer-right">
        <img src="../assets/dc-logo-bg.png" alt="Big Logo">
    </div>

    <div class="footer-bottom-banner">
        <div class="footer-left">
            <button><a href="#" id="button">SIGN UP NOW</a></button>
        </div>
        <ul class="menu-row footer-right">
            <li><a href="#" target="_blank" rel="noopener" id="follow">FOLLOW US</a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/footer-facebook.png" alt=""></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/footer-twitter.png" alt=""></a></li>            
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/footer-youtube.png" alt=""></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/footer-pinterest.png" alt=""></a></li>
            <li><a href="#" target="_blank" rel="noopener"><img src="../assets/footer-periscope.png" alt=""></a></li>
        </ul>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'FooterComponent',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



* {
    padding: 0;
    margin: 0;
    text-align: left;
    color: #fff;

}

.full-footer-container {
    position: relative;
}

.footer-container {
    display: flex;
    justify-content: space-around;
    background-image: url("../assets/footer-bg.jpg");
    height: 400px;
}

.footer-left {
    display: flex;
    width: 40%;
    padding: 5% 0 5% 15%;
}

.menu-col {
    display: flex;
    flex-direction: column;
}

.footer-right {
    width: 60%;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items:center;
}

.footer-right img {
    max-height: 400px;
    padding-left: 5%;
}

.footer-left h6 {
    padding: 10px;
    margin-top: 10px;
}

.footer-left ul {
  list-style-type: none;
  padding: 0;
  margin-top: 10px;
}

.footer-left li {
  display: inline-block;
  margin: 0 10px;
  font-size: 11px;
  vertical-align: center;
  padding: 1% 0;

}

a {
    text-decoration: none;
    color: #605f60
}

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
    color: #0c69f7;
}

.footer-right li {
  display: inline-block;
  margin: 0 5px;
  font-size: 11px;
  vertical-align: center;
  padding: 0;

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
}

#button {
    color: white;
}

/* shop container */

.shop-container {
    display: flex;
    justify-content: space-around;
    background-color: #0c69f7;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;

}

.shop-row {
    display: flex;
    justify-content: center;
    align-items: center;
}

.img-card {
    width: 40px;
    height: 40px;
}

.img-card img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    padding-right: 10px;
}

h6 {
    padding-left: 10px;
}




#shop-list {
    list-style-type: none;
    padding: 0;
    height: 100%;
    margin: auto;
    line-height: 70px;
    display: flex;
    align-self: center;
}
#shop-list li {
  display: inline-block;
  margin: 0 10px;
  font-size: 11px;
  font-weight: 600;
  vertical-align: center;
}
#shop-list a {
  color: #fff;
  text-decoration: none;
}



</style>