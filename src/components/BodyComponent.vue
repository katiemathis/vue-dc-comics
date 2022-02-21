<template>
  <div class="body-container">
    <div>
        <p>--> CONTENT GOES HERE  </p>
    </div>
  </div>
</template>

<script>
export default {
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
    
    p {
        line-height: 100px;
    }
}

</style>