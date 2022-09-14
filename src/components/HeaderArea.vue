<template>
  <v-container>
    <div class="header_bg">
      <div class="header_main d-flex justify-space-between">
        <h1>
          <a href="/">
            <img src="../assets/logo.png" alt="郝喫牛排" class="logo mx-3" />
          </a>
        </h1>

        <div class="header-nav d-flex align-center">
          <ul>
            <li class="mx-4" v-for="item in headerNav" :key="item.title">
              <a class="text-subtitle-2" href="">{{ item.title }}</a>
            </li>
          </ul>
          <div class="ml-4">
            <v-container>
              <v-row>
                <v-col cols="3 d-flex align-center">
                  <v-icon color="red accent-2">mdi-phone-in-talk</v-icon>
                </v-col>
                <v-col cols="9 text-subtitle-2">
                  <span class="phone-color">連絡電話：<br />02-1234567</span>
                </v-col>
              </v-row>
            </v-container>
          </div>
        </div>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "HeaderArea",
  data: () => ({
    headerNav: [
      {
        title: "首頁",
      },
      {
        title: "經營理念",
      },
      {
        title: "美味菜單",
      },
      {
        title: "聯絡我們",
      },
      {
        title: "分店資訊",
      },
    ],
  }),
};
</script>

<style lang="scss" scoped>
.header_bg {
  height: 68px;
  background-color: rebeccapurple;
  .header_main {
    margin: 0 auto;
    width: 1200px;
    height: 68px;
    background-color: #fff;
  }

  .logo {
    height: 60px;
  }
  .header-nav {
    & > ul > li {
      display: inline-block;
      & > a {
        color: #333;
      }
    }
    .phone-color {
      color: #ff5252;
    }
  }
}
</style>
