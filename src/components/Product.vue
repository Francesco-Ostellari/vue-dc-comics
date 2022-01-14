<template>
<div>
  <div class="container-card">
    <div class="thumb-img">
      <img :src="img" :alt="titolo">
    </div>
    <div class="text">
      <span>{{titolo}}</span>
    </div>
  </div>  
</div>
</template>

<script>
export default {  
  name: "Product",
  props: ['img', 'alt', 'titolo'],
}
</script>

<style lang="scss">
  .container-card {
    .thumb-img {
      width: 150px;
      height: 150px;
      overflow: hidden;
      img {
        width: 100%;
      }
    }
    .text {
      margin: 10px 0 20px 0;
      width: 150px;
      color: white;
      text-transform: uppercase;
      span {
        width: 100%;
        display: inline-block;
      }
    }
  }
</style>