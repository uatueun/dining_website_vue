<template>
  <div class="new-menu-area d-flex justify-center">
    <div class="new-menu-content d-flex align-center">
      <img src="@/assets/images/material1.png" alt="新菜單介紹" />

      <v-card
        class="new-menu-card"
        elevation="3"
        width="720"
        height="293"
        color="#fff"
        tile
      >
        <v-card-text class="my-8 px-8">
          <span class="text-h4 new-menu-title">新品推薦</span>

          <div class="text-body-2 text--primary pl-16 ml-6 mt-10">
            吃麻辣火鍋有一種吃法，那叫串串香！<br />
            源於四川成都的麻辣火鍋串串，就是用竹籤把各種肉食、蔬菜串成一串一串，再一把放入火鍋自己燙熟，吃完再叫老闆來數竹籤結帳，這種又好吃又好玩的吃法，這次來到重慶吃了一家串串界網紅店，不只體會到川渝麻辣的江湖味，更有巴蜀的文青味！
          </div>

          <a
            href="javascript;"
            class="text-subtitle-1 new-menu-more d-flex justify-end"
            >查看詳情 ></a
          >
        </v-card-text>
      </v-card>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.new-menu-area {
  height: 540px;
  position: relative;
  .new-menu-content {
    width: 1200px;
  }
  .new-menu-card {
    position: absolute;
    right: 540px;
    z-index: 1;
    .new-menu-title {
      padding-bottom: 10px;
      color: #ff5252;
      border-bottom: 3px solid #ff5252;
    }
    .new-menu-more {
      color: #ff5252;
    }
  }
}
</style>
