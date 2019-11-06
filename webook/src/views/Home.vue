<template>
  <div class="home container-full">
    <section class="banner p-0">
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
        <h1>— 我们的产品 —</h1>
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
                <b-button
                  href="#"
                  variant="link"
                  class="text-danger p-0 mt-2 text-decoration-none"
                >了解详情></b-button>
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
                <b-button
                  href="#"
                  variant="link"
                  class="text-danger p-0 mt-2 text-decoration-none"
                >了解详情></b-button>
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
                <b-button
                  href="#"
                  variant="link"
                  class="text-danger p-0 mt-2 text-decoration-none"
                >了解详情></b-button>
              </b-card-body>
            </b-card>
          </b-col>
          <b-col class="col-sm-6 col-md-4 col-12">1</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">2</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">3</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">4</b-col>
          <b-col class="col-sm-6 col-md-4 col-12">5</b-col>
        </b-row>
      </b-container>
    </section>
    <section class="people">
      <header>
        <h1>— 人人都是生活的作者 —</h1>
        <p>Everyone is author of life</p>
      </header>
      <b-container>
        <b-row class="mx-0 align-items-center">
          <b-col class="p-0 col-sm col-12">
            <b-img-lazy fluidGrow blank src="https://picsum.photos/700/450/?image=80" alt="Image 1"></b-img-lazy>
          </b-col>
          <b-col class="p-0 col-sm-4 col-12">
            <div class="info text-left">
              <div class="title">妈妈们</div>
              <div class="desc">随手发在朋友圈的宝宝日常照片和趣事，简单导出就是一本成长日记。</div>

              <b-button
                @click="previewImage"
                variant="link"
                class="small mt-2 text-decoration-none text-danger p-0"
              >查看更多</b-button>
            </div>
          </b-col>
        </b-row>
        <b-row class="mx-0 align-items-center flex-row-reverse">
          <b-col class="p-0 col-sm col-12">
            <b-img-lazy fluidGrow blank src="https://picsum.photos/700/450/?image=84" alt="Image 1"></b-img-lazy>
          </b-col>
          <b-col class="p-0 col-sm-4 col-12">
            <div class="info text-left">
              <div class="title">妈妈们</div>
              <div class="desc">随手发在朋友圈的宝宝日常照片和趣事，简单导出就是一本成长日记。</div>

              <b-button
                @click="previewImage"
                variant="link"
                class="small mt-2 text-decoration-none text-danger p-0"
              >查看更多</b-button>
            </div>
          </b-col>
        </b-row>
        <b-row class="mx-0 align-items-center">
          <b-col class="p-0 col-sm col-12">
            <b-img-lazy fluidGrow blank src="https://picsum.photos/700/450/?image=82" alt="Image 1"></b-img-lazy>
          </b-col>
          <b-col class="p-0 col-sm-4 col-12">
            <div class="info text-left">
              <div class="title">妈妈们</div>
              <div class="desc">随手发在朋友圈的宝宝日常照片和趣事，简单导出就是一本成长日记。</div>

              <b-button
                @click="previewImage"
                variant="link"
                class="small mt-2 text-decoration-none text-danger p-0"
              >查看更多</b-button>
            </div>
          </b-col>
        </b-row>
        <b-row class="mx-0 align-items-center flex-row-reverse">
          <b-col class="p-0 col-sm col-12">
            <b-img-lazy fluidGrow blank src="https://picsum.photos/700/450/?image=85" alt="Image 1"></b-img-lazy>
          </b-col>
          <b-col class="p-0 col-sm-4 col-12">
            <div class="info text-left">
              <div class="title">妈妈们</div>
              <div class="desc">随手发在朋友圈的宝宝日常照片和趣事，简单导出就是一本成长日记。</div>

              <b-button
                @click="previewImage"
                variant="link"
                class="small mt-2 text-decoration-none text-danger p-0"
              >查看更多</b-button>
            </div>
          </b-col>
        </b-row>
        <b-row class="mx-0 align-items-center">
          <b-col class="p-0 col-sm col-12">
            <b-img-lazy fluidGrow blank src="https://picsum.photos/700/450/?image=88" alt="Image 1"></b-img-lazy>
          </b-col>
          <b-col class="p-0 col-sm-4 col-12">
            <div class="info text-left">
              <div class="title">妈妈们</div>
              <div class="desc">随手发在朋友圈的宝宝日常照片和趣事，简单导出就是一本成长日记。</div>

              <b-button
                variant="link"
                class="small mt-2 text-decoration-none text-danger p-0"
                @click="previewImage"
              >查看更多</b-button>
            </div>
          </b-col>
        </b-row>
        <!-- 图片预览 -->
        <b-modal id="images-preview" hide-backdrop>
          <template v-slot:modal-header="{ close }">
            <b-button size="sm" variant="outline-danger" @click="close()">Close Modal</b-button>
          </template>
          <template v-slot:default="{ close }">
            <div class="preview-swiper-box">
              <div class="swiper-wrapper">
                <div class="swiper-slide">
                  <div
                    data-background="https://picsum.photos/1024/480/?image=55"
                    class="swiper-lazy swiper-img"
                    @click="close"
                  >
                    <div class="swiper-lazy-preloader"></div>
                  </div>
                </div>
                <div class="swiper-slide">
                  <div
                    data-background="https://picsum.photos/1024/480/?image=58"
                    class="swiper-lazy swiper-img"
                    @click="close"
                  >
                    <div class="swiper-lazy-preloader"></div>
                  </div>
                </div>
                <div class="swiper-slide">
                  <div
                    data-background="https://picsum.photos/1024/480/?image=52"
                    class="swiper-lazy swiper-img"
                    @click="close"
                  >
                    <div class="swiper-lazy-preloader"></div>
                  </div>
                </div>
              </div>
              <div class="preview-swiper-pagination"></div>
              <div class="swiper-button-prev"></div>
              <!--左箭头。如果放置在swiper-container外面，需要自定义样式。-->
              <div class="swiper-button-next"></div>
              <!--右箭头。如果放置在swiper-container外面，需要自定义样式。-->
            </div>
          </template>
        </b-modal>
      </b-container>
    </section>
    <section class="their-words">
      <header>
        <h1>— 他们说 —</h1>
        <div>Their words</div>
        <div>「这是一份比任何东西都让人期待和惊喜的礼物！」</div>
      </header>
      <b-container>
        <b-row class="justify-content-center">
          <b-col class="col-sm-3 col-6">
            <b-card
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="div"
              class="mb-2"
            >
              <b-card-text
                title="#Some quick example text to build#on the card title and make up the bulk of the card's content."
                class="card-info"
              >Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.</b-card-text>
              <b-card-text class="text-right">李磊</b-card-text>
            </b-card>
          </b-col>
          <b-col class="col-sm-3 col-6">
            <b-card
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="div"
              class="mb-2"
            >
              <b-card-text
                title="#Some quick example text to build#on the card title and make up the bulk of the card's content."
                class="card-info"
              >Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.</b-card-text>
              <b-card-text class="text-right">李磊</b-card-text>
            </b-card>
          </b-col>
          <b-col class="col-sm-3 col-6">
            <b-card
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="div"
              class="mb-2"
            >
              <b-card-text
                title="#Some quick example text to build#on the card title and make up the bulk of the card's content."
                class="card-info"
              >Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.</b-card-text>
              <b-card-text class="text-right">李磊</b-card-text>
            </b-card>
          </b-col>
          <b-col class="col-sm-3 col-6">
            <b-card
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="div"
              class="mb-2"
            >
              <b-card-text
                title="#Some quick example text to build#on the card title and make up the bulk of the card's content."
                class="card-info"
              >Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.Some quick example text to build on the card title and make up the bulk of the card's content.</b-card-text>
              <b-card-text class="text-right">李磊</b-card-text>
            </b-card>
          </b-col>
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
  methods: {
    previewImage() {
      this.$bvModal.show("images-preview");
      this.$nextTick(() => {
        let PreviewSwiper = new Swiper(".preview-swiper-box", {
          lazy: {
            loadPrevNext: true
          },
          direction: "horizontal",
          watchSlidesVisibility: true,
          observer: true, //修改swiper自己或子元素时，自动初始化swiper
          observeParents: true, //修改swiper的父元素时，自动初始化swiper
          //使用分页器
          pagination: {
            el: ".preview-swiper-pagination",
            bulletActiveClass: "bullet-active",
            clickable: true
          },
          navigation: {
            nextEl: ".swiper-button-next",
            prevEl: ".swiper-button-prev"
          }
        });
      });
    }
  },
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
.row .col {
  padding: 10px;
}
img {
  user-select: none;
}
section:not(.products) .container,
.row {
  padding: 0;
}
/deep/ #images-preview {
  padding: 0 !important;
  .modal-header,
  .modal-footer {
    display: none;
  }
  background-color: #222;
  .modal-dialog,
  .modal-content,
  .modal-body {
    max-width: none;
    display: block;
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    background-color: #222;
    color: white;
    .preview-swiper-box,
    .swiper-wrapper {
      position: relative;
      width: 100%;
      height: 100%;
    }
    .swiper-slide {
      position: relative;
      .swiper-img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        border-radius: 5px;
        background: no-repeat;
        background-size: 100%;
        background-position: 100%;
      }
    }
    .swiper-pagination-bullets {
      position: absolute;
      bottom: 20px;
      text-align: center;
    }
    .bullet-active {
      background: white;
      opacity: 1;
    }
  }
}
.home {
  position: relative;
  section {
    position: relative;
    padding: 3rem 1rem;
  }
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
  .people {
    .row {
      margin-top: 2rem;
      background-color: #f7f7f7;
      border-radius: 5px;
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
      font-size: 1.25em;
      overflow: hidden;
      .img-fluid {
        object-fit: cover;
        border-radius: 5px;
        width: 100%;
        height: 100%;
      }
      .info {
        font-size: 1.25rem;
        padding: 2rem;
        .title {
          background-color: rgb(200, 150, 102);
          display: inline-block;
          color: #fff;
          margin-bottom: 0.5em;
          padding: 0.25rem 1rem;
          border-radius: 100px;
        }
        .desc {
          color: rgb(200, 150, 102);
        }
      }
    }
    .row:nth-of-type(1) {
      margin-top: 0;
    }
  }
  .their-words {
    .card-info {
      overflow: hidden;
      display: -webkit-box;
      -webkit-box-orient: vertical;
      -webkit-line-clamp: 3;
    }
  }
}
@media (max-width: 575px) {
  .card-img-top {
    border-top-right-radius: 0;
  }
  .card-body {
    text-align: left;
  }
  section:not(.their-words) .row .col {
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
@media (max-width: 1200px) {
  h1 {
    font-size: calc(1.375rem + 1.5vw);
  }
}
</style>
