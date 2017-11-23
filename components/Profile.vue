<template>
  <section class = "content">
    <p class="myPhoto"><img src="/myProfile.png"></p>
    <h2 class="title">
      HELLO
      <p class="name">I'm Yurie Yajima</p>
    </h2>

    <p class="role">Frontend Engineer / Web Director / Planner</p>
    <p class="disc">ユーザにとっての最高の状態を作るために、問題解決を進めるのが得意です。</p>
  </section>
</template>

<style scoped>
  .content {
    padding: 42px;
    background-image: url('../static/contentBg02.png');
  }
  .myPhoto {
    margin-top: -107px;
  }
  .title {
    font-size: 48px;
    color: #863461;
    margin: 21px 0 7px;
  }
  .name {
    font-size: 24px;
    font-weight: 600;
    color: #000;
    margin-bottom: 35px;
  }
  .role {
    font-size: 14px;
    margin-bottom: 7px;
  }
  .disc {
    font-size: 12px;
    font-weight: 300;
    margin-bottom: 35px;
  }
</style>
