<template>
    <div class="container">
        <button id="top"><a href="#">CURRENT SERIES</a></button>
        <div class="product-cards-container">
            
            <div class="product-cards"
                v-for="(product, index) in products" :key="index">
                <!--:class="(product[index <12])?'show':'hide'"-->
                <div class="product-card">
                    <div class="product-image">
                        <img href="#" :src="product.thumb">
                    </div>
                    <div class="product-series">
                        <h6>{{product.series}}</h6>
                    </div>
                </div>
            
            </div>
        </div>
        <button id="bottom"><a href="#">LOAD MORE</a></button>
        
    </div>

          <!-- <div v-if="showLess">
          <div v-for="(value,index) in object">
          <template v-if="index <= 5"></template>
            </div>
          </div> 
          <div v-else> 
          <div v-for="value in object"></div>
          </div> 
          <button @click="showLess = false"></button>-->




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

.container {
    width: 100%;
    position: absolute;
    height: 700px;
    background-color: black;
    padding: 20px 0;

    #top {
    @include blue-button;
    position: absolute;
    left: 250px;
    top: -40px;
    font-size: x-small;
    &:hover {
      background-color: $colorWhite;
      }

        a {
          text-decoration: none;
          padding: 10px 20px;
          color: $colorWhite;
          &:hover {
            color: #000;
          }
        }
    }


    .product-cards-container {
        @include flex-row-around;
        flex-wrap: wrap;
        margin-bottom: 10px;
        width: 60%;
        margin: auto;
        

        .product-cards {
            @include flex-row-around;
            height: 150px;

            .product-card {
                @include flex-column;
                height: 150px;
                width: 100px;
                margin: 10px;
                &:hover {
                    cursor: pointer;
                }

                .product-image {
                    height: 100px;
                    width: 100px;
                
                        img {
                            width: 100%;
                            height: 100%;
                            object-fit: cover;
                            &:hover {
                                border: 2px $colorWhite solid;
                                cursor: pointer;
                            }
                        }
                }

                .product-series {
                    margin-top: 5px;
                    padding-top: 5px;
                    width: 100%;
                    vertical-align: middle;
                    text-transform: uppercase;
                    font-size: xx-small;
                    
                }

            }

        }

      
    }
    #bottom {
      @include blue-button;
      margin-left: 45%;
      &:hover {
      background-color: $colorWhite;
      }

        a {
          text-decoration: none;
          padding: 10px 20px;
          color: $colorWhite;
          font-size:xx-small;
          &:hover {
            color: #000;
          }
        }
      
    }
 
}

</style>