<template>
  <footer>
    <div class="footer-top">
      <div class="sfondo">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
      <div class="container-footer-top flex">
        <div class="col-left">
          <ul>
            <li> 
              <h1>
                dc comics
              </h1> 
            </li>
            <li>
              <a href="#">
                Characters 
              </a>
            </li>
            <li>
              <a href="#">
                Comics 
              </a>
            </li>
            <li>
              <a href="#">
                Movies 
              </a>
            </li>
            <li>
              <a href="#">
                TV 
              </a>
            </li>
            <li>
              <a href="#">
                Games 
              </a>
            </li>
            <li>
              <a href="#">
                Videos 
              </a>
            </li>
            <li>
              <a href="#">
                News 
              </a>
            </li>
          </ul>
          <ul>
            <li>
              <h1>
                shop
              </h1>
            </li>
              <li>
              <a href="#">
                Shop DC 
              </a>
            </li>
              <li>
              <a href="#">
                Shop DC Collectibles
              </a>
            </li>
          </ul>
        </div>
        <div class="col-center">
          <ul>
            <li>
              <h1>
                dc
              </h1>
            </li>
            <li>
              <a href="#">
                Terms of Use
              </a>
            </li>
            <li>
              <a href="#">
                Privacy policy (New)
              </a>
            </li><li>
              <a href="#">
                Ad Choices
              </a>
            </li><li>
              <a href="#">
                Advertising
              </a>
            </li><li>
              <a href="#">
                Job
              </a>
            </li><li>
              <a href="#">
                Subscriptions
              </a>
            </li><li>
              <a href="#">
                Talent Workshops
              </a>
            </li><li>
              <a href="#">
                CPSC Certificates
              </a>
            </li><li>
              <a href="#">
                Ratings
              </a>
            </li><li>
              <a href="#">
                Shop Help
              </a>
            </li><li>
              <a href="#">
                Contact Us
              </a>
            </li>
          </ul>
        </div>
        <div class="col-right">
          <ul>
            <li>
              <h1>
                sites
              </h1>
            </li>
            <li>
              <a href="#">
                DC
              </a>
            </li>
            <li>
              <a href="#">
                MAD Magazine
              </a>
            </li>
            <li>
              <a href="#">
                DC Kids
              </a>
            </li>
            <li>
              <a href="#">
                DC Universe
              </a>
            </li>
            <li>
              <a href="#">
                DC Power Visa
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container-footer-bottom flex">
        <button>
          sign-up now!
        </button>
        <div class="right-footer">
          <span>
            follow us
          </span>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </footer>
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
  footer {
    height: 450px;  
    .footer-top{
      position: relative;
      background-image: url('../assets/img/footer-bg.jpg');
      height: 100%;
      width: 100%;
      background-repeat: no-repeat;
      background-size: cover;
      padding: 60px 0;

      .sfondo {
        position: absolute;
        right: 300px;
        transform: translate(0%, -20%);
      }

      .container-footer-top {
        width: 70%;
        margin: 0 auto;
        .col-left, .col-center, .col-right {
          margin-right: 60px;
          ul {
            margin-bottom: 30px;
            list-style: none;
            li {
              a {
                text-decoration: none;
                color: white;
                font-weight: 200;
                margin-bottom: 5px;
                display: inline-block;
              }
              h1 {
                text-transform: uppercase;
                color: white;
                margin-bottom: 20px;
              }
            }
          }
        }
      }
    }
    .footer-bottom {
      background-color: #282828;
      padding: 30px 0;
      z-index: 999;
      .container-footer-bottom {
        width: 70%;
        margin: 0 auto;
        justify-content: space-between;
        align-items: center;
        text-transform: uppercase;
        button {
          text-transform: uppercase;
          padding: 15px;
          border-color: #0282F9;
          background-color: transparent;
          color: white;
          font-size: 1.2em;
        }
        .right-footer {
          span {
            color: #0282F9;
            font-weight: bold;
            margin-right: 15px;
          }
          img {
            vertical-align: middle;
            margin: 0 7px;
          }
        }
      }
    }
  }

  .flex {
    display: flex;
  }
</style>