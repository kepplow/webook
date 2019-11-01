<template>
  <div class="home container-full">
    <section class="banner">
      <div class="swiper-box">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <div
              data-background="https://picsum.photos/1024/480/?image=55"
              class="swiper-lazy swiper-img"
            >
              <div class="swiper-lazy-preloader"></div>
            </div>
          </div>
          <div class="swiper-slide">
            <div
              data-background="https://picsum.photos/1024/480/?image=58"
              class="swiper-lazy swiper-img"
            >
              <div class="swiper-lazy-preloader"></div>
            </div>
          </div>
          <div class="swiper-slide">
            <div
              data-background="https://picsum.photos/1024/480/?image=52"
              class="swiper-lazy swiper-img"
            >
              <div class="swiper-lazy-preloader"></div>
            </div>
          </div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
    </section>
    <section class="products">
      <header>
        <h1>—我们的产品—</h1>
        <p>Our Products</p>
      </header>
      <b-container class="text-sm-center">
        <b-row class="justify-content-center">
          <b-col class="col-sm-6 col-md-4 col-12">
            <b-card no-body tag="div" class="flex-row flex-sm-column align-items-center">
              <a href="#" class="w-100">
                <b-card-img-lazy src="https://picsum.photos/400/400/?image=20" top alt="Image"></b-card-img-lazy>
              </a>
              <b-card-body class="py-sm-4">
                <h4>微信书</h4>
                <div>微信从此跃然纸上</div>
                <b-button href="#" variant="link" class="text-danger p-0 mt-2">了解详情></b-button>
              </b-card-body>
            </b-card>
          </b-col>
          <b-col class="col-sm-6 col-md-4 col-12">
            <b-card no-body tag="div" class="flex-row flex-sm-column align-items-center">
              <a href="#" class="w-100">
                <b-card-img-lazy src="https://picsum.photos/400/400/?image=20" top alt="Image"></b-card-img-lazy>
              </a>
              <b-card-body class="py-sm-4">
                <h4>微信书</h4>
                <div>微信从此跃然纸上</div>
                <b-button href="#" variant="link" class="text-danger p-0 mt-2">了解详情></b-button>
              </b-card-body>
            </b-card>
          </b-col>
          <b-col class="col-sm-6 col-md-4 col-12">
            <b-card no-body tag="div" class="flex-row flex-sm-column align-items-center">
              <a href="#" class="w-100">
                <b-card-img-lazy src="https://picsum.photos/400/400/?image=20" top alt="Image"></b-card-img-lazy>
              </a>
              <b-card-body class="py-sm-4">
                <h4>微信书</h4>
                <div>微信从此跃然纸上</div>
                <b-button href="#" variant="link" class="text-danger p-0 mt-2">了解详情></b-button>
              </b-card-body>
            </b-card>
          </b-col>
          <b-col class="col-sm-6 col-md-4 col-12">1</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">2</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">3</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">2</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">3</b-col>
        </b-row>
      </b-container>
    </section>
  </div>
</template>

<script>
import "swiper/css/swiper.min.css";
import Swiper from "swiper";
export default {
  name: "home",
  data() {
    return {
      slide: 0,
      sliding: null
    };
  },
  methods: {},
  mounted() {
    var mySwiper = new Swiper(".swiper-box", {
      lazy: {
        loadPrevNext: true
      },
      direction: "horizontal",
      watchSlidesVisibility: true,
      observer: true, //修改swiper自己或子元素时，自动初始化swiper
      observeParents: true, //修改swiper的父元素时，自动初始化swiper
      //使用分页器
      pagination: {
        el: ".swiper-pagination",
        bulletActiveClass: "bullet-active",
        clickable: true
      },
      autoplay: {
        delay: 5000,
        disableOnInteraction: true //触碰后自动切换停止
      }
    });
  }
};
</script>
<style lang="less" scoped>
section {
  position: relative;
}
.row .col {
  padding: 10px;
}
.home {
  position: relative;
  .banner {
    .swiper-slide {
      position: relative;
      .swiper-img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-size: cover;
        border-radius: 5px;
      }
    }
    .swiper-slide:before {
      content: "";
      display: block;
      padding-top: 37.5%;
    }
    /deep/.swiper-pagination-bullet {
      background: #f56368;
      opacity: 0.2;
    }
    /deep/.bullet-active {
      background: #f56368;
      opacity: 1;
    }
  }
  .products {
    padding: 42px 14px 56px;
    .card {
      border: 0;
      box-shadow: 0 12px 40px hsla(0, 0%, 68.6%, 0.2);
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 20px;
      .card-img-top {
        object-fit: cover;
        transition: 0.3s;
      }
      .card-body {
        h4 {
          font-size: calc(1.275rem + 0.3vw);
        }
        min-width: 11em;
      }
    }
  }
}
@media (max-width: 575px) {
  .card-body {
    text-align: left;
  }
  .row .col {
    padding: 0;
  }
}
@media (min-width: 767.98px) {
  .home {
    margin-top: -56px;
  }
}
@media (max-width: 640px) {
  .home .banner .swiper-slide:before {
    content: "";
    display: block;
    padding-top: 57.25%;
  }
}
</style>
