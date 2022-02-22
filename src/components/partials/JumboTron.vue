<template>
    <div class="container">
    </div>
</template>

<script>
export default {
  name: 'JumboTron',

}
</script>

<style scoped lang="scss">

@import '../../assets/style/variables.scss';

.container {
    width: 100%;
    min-height: 300px;
    position: absolute;
    top: 20%;
    left: 0;
    background-color: #000;
    z-index: 9999;
}
