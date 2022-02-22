<template>
  <div class="shop-container">
        <ul>
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
</template>

<script>
export default {
  name: 'ShopBanner',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.shop-container {
    display: flex;
    justify-content: space-around;
    background-color: #0c69f7;

}

.shop-row {
    display: flex;
    justify-content: center;
    align-items: center;
}

.img-card {
    width: 50px;
    height: 50px;
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




ul {
    list-style-type: none;
    padding: 0;
    height: 100%;
    margin: auto;
    line-height: 70px;
    display: flex;
    align-self: center;
}
li {
  display: inline-block;
  margin: 0 10px;
  font-size: 11px;
  font-weight: 600;
  vertical-align: center;
}
a {
  color: #fff;
  text-decoration: none;
}
</style>