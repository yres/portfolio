<template>
  <section class = "content">
    <h2 class="title">SKILLS</h2>
    <div class="bars">
      <div class="bar">
        <p class="level5 clear"></p>
        <p class="level4"></p>
        <p class="level3"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">HTML</p>
      </div>
      <div class="bar">
        <p class="level5 clear"></p>
        <p class="level4"></p>
        <p class="level3"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">CSS</p>
      </div>
      <div class="bar">
        <p class="level5 clear"></p>
        <p class="level4 clear"></p>
        <p class="level3"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">JavaScript</p>
      </div>
      <div class="bar">
        <p class="level5 clear"></p>
        <p class="level4"></p>
        <p class="level3"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">運用力</p>
      </div>
      <div class="bar">
        <p class="level5"></p>
        <p class="level4"></p>
        <p class="level3"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">企画力</p>
      </div>
      <div class="bar">
        <p class="level5 clear"></p>
        <p class="level4 clear"></p>
        <p class="level3 clear"></p>
        <p class="level2"></p>
        <p class="level1"></p>
        <p class="text">マネジメント</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .content {
    padding: 56px 0;
    background-image: url('../static/contentBg01.png');
  }
  .title {
    font-size: 48px;
    margin-bottom: 35px;
    color: #fff;
  }
  .bars {
    padding: 0 32px 35px;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    margin: 0 auto;
    width: 60%;
  }
  .bar {
    width: 100px;
    height: 100%;
    position: relative;
    margin: 0 10px;
  }
  .bar p{
    margin-bottom: 7px;
    border-radius: 2px;
  }
  .level1 {
    margin: 0 auto;
    width: 30px;
    background: #DE9839;
    height: 30px;
  }
  .level2 {
    margin: 0 auto;
    width: 30px;
    background: #B04556;
    height: 30px;
  }
  .level3 {
    margin: 0 auto;
    width: 30px;
    background: #805D8D;
    height: 30px;
  }
  .level4 {
    margin: 0 auto;
    width: 30px;
    background: #785093;
    height: 30px;
  }
  .level5 {
    margin: 0 auto;
    width: 30px;
    background: #403A6D;
    height: 30px;
  }
  .clear {
    opacity: 0;
  }
  .text {
    color: #fff;
    margin: 14px 0;
    font-size: 12px;
    font-weight: 600;
  }
</style>
