<template>
        <div class="product-cards-container" >
            <div class="product-cards" v-for="(product, y) in products" :key="y">
                <div class="product-card">
                    <div class="product-image">
                        <img :src="product.thumb">
                    </div>
                    <div class="product-series">
                        <h6>{{product.series}}</h6>
                    </div>

                
                </div>
            
            </div>
            </div>
            <!--<div class="shop-container">
                    <ul id="shop-list">
                        <li v-for="(product, y) in products" :key="y">
                            <a href="#" target="_blank" rel="noopener" class="shop-row">
                                <div class="img-card">
                                    <img :src="product.src"> 
                                </div>
                                <h6>{{product.text}}</h6>
                            </a>

                        </li>
                    </ul>
            </div>-->
</template>

<script>


export default {
  name: 'ProductsSection',
  props: ["products"],

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../../assets/style/variables.scss';

* {
    @include body-rules;
    text-align: left;
    color: #fff;
}

.product-cards-container {
      @include flex-row-around;
      flex-wrap: wrap;
      width: 60%;
      margin: auto;

    
      .product-cards {
        @include flex-row-around;
        height: 150px;
        margin: auto;

          .product-card {
            @include flex-column;
            height: 100px;
            width: 100px;
            margin: 10px;

              .product-image {
                height: 100px;
                width: 100px;
            
                    img {
                        width: 100%;
                        height: 100%;
                        object-fit: cover;
                    }
              }

              .product-series {
                width: 100%;
                line-height: 50px;
              }

          }

      }
    }

</style>