<template>
  <div class="body-container">
    <JumboTron />
  </div>
</template>

<script>
import JumboTron from './partials/JumboTron.vue'
export default {
  components: { JumboTron },
  name: 'BodyComponent',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';

* {
  @include body-rules;
}

.body-container {
    background-color: #000;
    color: $colorWhite;
    font-size: 16px;
    font-weight: 600;
    min-height: 100px;
    background-image: url("../assets/img/jumbotron.jpg");
    
}

</style>