<template>
  <main>
    <div class="main-top flex">
      <div class="container-main-top">
        <h1>--> Content goes here </h1>
      </div>
    </div>
    <div class="main-bottom flex">
      <div class="container-main-bottom">
        <ul class="flex">
          <li>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <span> digital comics </span>
          </li>
          <li>
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <span> dc merchandise </span>
          </li>
          <li>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <span> subscription </span>
          </li>
          <li>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <span> comic shop locator </span>
          </li>
          <li>
            <img class="svg" src="../assets/img/buy-dc-power-visa.svg" alt="">
            <span> dc power visa </span>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Main',
  data() {
    return {
      
    }
  }
}
</script>

<style lang="scss" scoped>
  main {
    .main-top {
      background-color: #1A1A1A;
      height: 150px;
      align-items: center;
        .container-main-top{
          width: 70%;
          margin: 0 auto;
          h1 {
            color: white;
          }
        }
    }
    .main-bottom {
      background-color: #0282F9;
      height: 200px;
      align-items: center;
      justify-content: space-around;
      .container-main-bottom {
        width: 70%;
        margin: 0 auto;
        justify-content: space-between;
        ul {
          justify-content: space-between;
          align-items: center;
          li {
            display: inline-block;
            img {
              height: 80px;
              vertical-align: middle;
              margin-right: 10px;
            }
            span {
              text-transform: uppercase;
              color: white;
            }
            .svg {
              height: 65px;
            }
          }
        } 
      }
    }
  }

  .flex {
    display: flex;
  }
</style>