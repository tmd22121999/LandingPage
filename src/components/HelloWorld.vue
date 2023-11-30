<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>Trang web đang được thực hiện</h1>

  <div class="card text-white">
    <!-- <button type="button" @click="count++">count is {{ count }}</button> -->
    <p>Trang web của 99's Studio, nhóm làm game idle nhỏ tại Việt Nam</p>
    https://tmd22121999.github.io/99s-Studio
  </div>

  <p>
    Mời bạn chơi thử game đầu tay do nhóm thực hiện :
    <a href="https://ngocquang269.itch.io/the-transporter" target="_blank"
      >The Transporter</a
    >
  </p>
  <!-- <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p> -->
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
