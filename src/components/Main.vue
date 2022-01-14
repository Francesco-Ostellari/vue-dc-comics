<template>
  <main>
    <div class="jumbotron">
    </div>
    <div class="main-top flex">
      <div class="container-main-top" >
        <div class="title">
          <h1>current series</h1>
        </div>
        <div class="container-img flex">
          <Product
            v-for="(thumb, index) in thumbs"
            :key="index"
            :img="thumb.thumb"
            :alt="thumb.series"
            :titolo="thumb.series"
          />
        </div>
        <div class="container-button flex">
          <div class="button">
            load more
          </div>
        </div>
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
import Product from './Product.vue'
export default {
  name: 'Main',
  components: {
    Product,
  },
  data() {
    return {
      thumbs: [
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book"
        },
        {
          thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
  main {
    .jumbotron {
      background-image: url('../assets/img/jumbotron.jpg');
      background-size: cover;
      padding: 300px 0;
    }
    .main-top {
      background-color: #1A1A1A;
        .container-main-top{
          width: 70%;
          margin: 0 auto;
          position: relative;
          .title {
            position: absolute;
            transform: translate(0%, -50%);
            background-color: #0282F9;
            width: 300px;
            padding: 5px 0;
            z-index: 999;
            h1 {
              color: white;
              text-transform: uppercase;
              text-align: center;
              z-index: 999;
            }
          }
          .container-img {
            padding: 50px 0;
            flex-wrap: wrap;
            gap: 20px;
          }
          .container-button {
            justify-content: center;
            margin-bottom: 10px;
            .button {
              background-color: #0282F9;
              width: 200px;
              padding: 10px 0;
              text-align: center;
              color: white;
              text-transform: uppercase;
              font-weight: bold;
            }
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