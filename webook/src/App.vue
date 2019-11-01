<template>
  <main id="app">
    <header>
      <b-navbar toggleable="md" type="light" class="site-nav">
        <b-navbar-brand href="#">岑泽网络科技</b-navbar-brand>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="/" active>首页</b-nav-item>
          <b-nav-item href="/order">订单</b-nav-item>
          <b-nav-item href="#">书架</b-nav-item>
          <b-nav-item href="#">晒单</b-nav-item>
          <b-nav-item href="#">
            <span>Rose</span>
          </b-nav-item>
        </b-navbar-nav>
      </b-navbar>
      <b-navbar type="light" class="bottom-nav" fixed="bottom">

        <!-- Right aligned nav items -->
        <b-navbar-nav class="container">
          <b-nav-item href="/" active>首页</b-nav-item>
          <b-nav-item href="/order">订单</b-nav-item>
          <b-nav-item href="#">书架</b-nav-item>
          <b-nav-item href="#">晒单</b-nav-item>
          <b-nav-item href="#">
            <span>我的</span>
          </b-nav-item>
        </b-navbar-nav>
      </b-navbar>
    </header>
    <div class="wrapper">
      <router-view />
    </div>
    <footer>这是尾部</footer>
  </main>
</template>

<style lang="less">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html,body {
  font-size: 14px;
  background-color: aliceblue;
  overflow-x: hidden;
}
.site-nav {
  position: relative;
  z-index: 20;
}
.bottom-nav {
  z-index: 20;
  background: #fff;
  transition: 0.3s;
  border-top: 1px solid rgba(0,0,0,.1);
  box-shadow: 0 2px 4px rgba(50,50,50,.1);
}
.navbar-light .navbar-nav .nav-link.active, .navbar-light .navbar-nav .nav-link:hover{
  color: #f56368;
}
footer {
  height: 300px;
  border: 1px solid rgba(0, 0, 0, 0.5);
}
@media (max-width: 767.98px) {
  .site-nav {
    display: none;
  }
  footer {
    display: none;
  }
}
@media (min-width: 576px) {
  .bottom-nav {
    display: none;
  }
}
</style>
