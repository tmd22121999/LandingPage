<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a class="navbar-brand" href="#">Game Studio X</a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#about">Giới Thiệu</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#games">Danh Sách Game</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#contact">Liên Hệ</a>
        </li>
      </ul>
    </div>
  </nav>

  <section id="hero" class="jumbotron text-center">
    <div class="container">
      <h1 class="display-4">Chào mừng bạn đến với Game Studio X</h1>
      <p class="lead">Nâng tầm trải nghiệm game với những tác phẩm độc đáo và đa dạng từ chúng tôi.</p>
      <a class="btn btn-primary btn-lg" href="#games" role="button">Xem Danh Sách Game</a>
    </div>
  </section>

  <section id="about" class="container my-5">
    <div class="row">
      <div class="col-lg-6">
        <h2>Về Chúng Tôi</h2>
        <p>
          Chúng tôi là một đội ngũ đam mê và sáng tạo, tập trung vào việc phát triển những trải nghiệm game độc đáo và
          không ngừng đổi mới.
        </p>
      </div>
      <div class="col-lg-6">
        <!-- Thêm hình ảnh hoặc video giới thiệu về studio game -->
      </div>
    </div>
  </section>

  <section id="games" class="bg-light py-5">
    <div class="container text-center">
      <h2>Danh Sách Game</h2>
      <!-- Thêm danh sách các game và thông tin chi tiết -->
    </div>
  </section>
  <section id="game2" class="bg-light py-5" style="width: 100vw; height: 200px; translate: -150px">
    <div class="">
      <div id="object"></div>
      <!-- Thêm danh sách các game và thông tin chi tiết -->
    </div>
  </section>
  <section id="lorem" class="container my-5 text-center">
    <div class="row mx-auto" style="max-width: 500px; text-align: center">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
      magna aliqua. Pharetra massa massa ultricies mi quis. Quam pellentesque nec nam aliquam sem et tortor. Morbi
      tristique senectus et netus et malesuada. Aliquet bibendum enim facilisis gravida neque. Tincidunt tortor aliquam
      nulla facilisi. Turpis egestas sed tempus urna. Fringilla ut morbi tincidunt augue. Morbi leo urna molestie at
      elementum. Mauris a diam maecenas sed enim. Ullamcorper eget nulla facilisi etiam dignissim diam quis. Felis
      bibendum ut tristique et.
    </div>
  </section>
  <section id="contact" class="container my-5">
    <div class="row">
      <div class="col-lg-6">
        <h2>Liên Hệ</h2>
        <!-- Thêm thông tin liên hệ -->
      </div>
      <div class="col-lg-6">
        <!-- Thêm biểu mẫu liên hệ hoặc thông tin khác -->
      </div>
    </div>
  </section>

  <footer class="text-center py-3">
    <p>&copy; 2023 Game Studio X. All rights reserved.</p>
  </footer>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
#game2 {
  background-image: url("../assets/street-Sheet.png");
}
#object {
  background-image: url("../assets/bike.png");
  width: 50px;
  height: 50px;
  transform: translateX(0vw);
  animation: scroll-watcher linear;
  animation-timeline: view();
}
@keyframes scroll-watcher {
  to {
    transform: translateX(100vw);
  }
}
</style>
