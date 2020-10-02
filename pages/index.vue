<template>
  <div class="home">
    <h1>Sho Matsubara</h1>
    <div class="menu-top">
      <ul>
        <li>About</li>
        <li>Works</li>
        <li>Skill</li>
        <li>Contact</li>
      </ul>
    </div>
    <div class="header-img">
      <img src="~/assets/img/header1.jpg" alt="自分の写真とテキスト">
    </div>
    <div class="works">
      <h2>Works</h2>
        <ul>
          <li>
            <img src="~/assets/img/work1.png" alt="住宅ローンシミュレーション">
          </li>
          <li>
            <img src="~/assets/img/comingsoon.jpeg" alt="">
          </li>
          <li>
            <img src="~/assets/img/comingsoon.jpeg" alt="">
          </li>
        </ul>
    </div>
    <div class="skill">
      <h2>Skill</h2>
      <div class="skill-catalog">
        <ul>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/htmlcss.jpeg" alt="HTML CSSのロゴ" width="120px" height="120px">
              <div class="skill-catalog-contens-text">
                <h3>HTML5/CSS3</h3>
                <p>SCSSを含め、基本的なコーディングは問題ありません。<br>レスポンシブやBEMは現在勉強中です。</p>
              </div>
            </div>
          </li>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/vuejs.png" alt="Vue.jsのロゴ" width="120px">
              <div class="skill-catalog-contens-text">
                <h3>Vue.js</h3>
                <p>シンプルな構造のアプリケーション作成ができます。</p>
              </div>
            </div>
          </li>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/photoshop.png" alt="Photoshopのロゴ" width="120px">
              <div class="skill-catalog-contens-text">
                <h3>Photoshop</h3>
                <p>基本的な操作は検索しながらできるレベルで、現在勉強中です。</p>
              </div>
            </div>
          </li>
        </ul>
        <ul>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/js.png" alt="JavaScriptのロゴ" width="120px">
              <div class="skill-catalog-contens-text">
                <h3>JavaScript</h3>
                <p>簡単なアニメーションをつけることができます。</p>
              </div>
            </div>
          </li>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/nuxt.png" alt="Nuxt.jsのロゴ" width="120px">
              <div class="skill-catalog-contens-text">
                <h3>Nuxt.js</h3>
                <p>Vue.js同様、シンプルなアプリケーションの作成ができます。</p>
              </div>
            </div>
          </li>
          <li>
            <div class="skill-catalog-contents">
              <img src="~/assets/img/firebase.png" alt="Firebaseのロゴ" width="120px">
              <div class="skill-catalog-contens-text">
                <h3>Firebase</h3>
                <p>認証・CRUDの実装ができます。</p>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="blog">
      <h2>blog</h2>
      <div class="blog-catalog">
        <ul>
          <li>
            <instagram-embed 
              :url="'https://www.instagram.com/p/BvF_xt_gwp-/'"
              :hide-caption="true"
            />
          </li>
          <li>
            <instagram-embed 
              :url="'https://www.instagram.com/p/BbZRtZiFcBf/'"
              :hide-caption="true"
            />
          </li>
          <li>
            <instagram-embed 
              :url="'https://www.instagram.com/p/BvDoxraAXSd/'"
              :hide-caption="true"
            />
          </li>
        </ul>
      </div>
    </div>
    <div class="logo-img">
      <img src="~/assets/img/icon_totop.gif" alt="トップにアップするためのロゴ">
    </div>
    <div class="menu-bottom">
      <ul>
        <li>About</li>
        <li>Works</li>
        <li>Skill</li>
        <li>Contact</li>
      </ul>
      <p>© ShoMatsubara All rights reserved.</p>
    </div>
  </div>
</template>

<script>
export default {
  components: {
  },
  data() {
    return {
    }
  }
};
</script>

<style lang="scss">
@import "@/assets/style/reset.css";

.home{
  margin: 98px auto;
  width: 1020px;
  > h1 {
    font-weight: 800;
    font-size: 2.5rem;
    margin-bottom: 32px;
  }
  .menu-top {
    ul {
      display: flex;
      float: right;
      width: 400px;
      li {
        width: 78px;
        margin: 0 auto;
      }
    }
  }
  .header-img {
    img {
      margin: 64px auto 100px;
      width: 100%;
    }
  }
  h2 {
    margin-bottom: 24px;
    font-weight: 400;
    font-size: 2rem;
    text-align: center;
  }
  .works{
    margin-bottom: 130px;
    ul {
      display: flex;
      li {
        border: solid 1px lightgray;
        width: 300px;
        height: 250px;
        background: skyblue;
        margin: 0 auto;
        img {
          width: 100%;
          height: 100%;
        }
      }
    }
  }
  .skill {
    margin-bottom: 130px;
    .skill-catalog {
      display: flex;
      ul {
        margin: 0 auto;
        padding-left: 16px;
        li {
          width: 450px;
          height: 150px;
          margin-bottom: 32px;
          .skill-catalog-contents {
            justify-content: end;
            display: flex;
            .skill-catalog-contens-text {
              margin-left: 16px;
              h3 {
                font-weight: 600;
                font-size: 1.2rem;
                padding-bottom: 12px;
                }
              p {
                line-height: 1.5;
              }
            }
          }
        }
      }
    }
  }
  .blog {
    .blog-catalog {
      margin-bottom: 98px;
      ul {
        display: flex;
        margin: 0 auto;
        li {
          width: 350px;
        }
      }
    }
  }
  .logo-img {
    text-align: center;
    margin-bottom: 64px;
    img {
      width: 22px;
      height: 14px;
    }
  }
  .menu-bottom {
    margin-bottom: 130px;
    ul {
      display: flex;
      float: left;
      width: 400px;
      li {
        width: 78px;
        margin: 0 auto;
      }
    }
    p {
      float: right;
      font-weight: 300;
      font-size: 12px;
      letter-spacing: -0.8px;
    }
  }
  .Header {
    display: none;
      .AvatarContainer {
        display: none;
      }
  }
}
</style>
