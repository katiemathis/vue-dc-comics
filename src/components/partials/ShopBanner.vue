<template>
  <div class="shop-container">
        <ul id="shop-list">
            <li v-for="(item,index) in items" :key="index">
                <a href="#" target="_blank" rel="noopener" class="shop-row">
                    <div class="img-card">
                        <img :src="item.src"> 
                    </div>
                    <h6>{{item.text}}</h6>
                </a>

            </li>
        </ul>
  </div>
</template>

<script>


export default {
  name: 'ShopBanner',
  props: ["items"],

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
            padding: 0 5px;
            &:hover {
                background-color: rgba(0,0,0,0.5);
                cursor: pointer;
            }

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

</style>