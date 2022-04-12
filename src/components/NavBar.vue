<template>
  <header :class="{ 'scrolled-nav': scrollPos }">
    <nav>
      <div class="branding">
        <img src="@/assets/icon.png" alt="" />
      </div>
      <ul class="navigation">
        <li>
          <router-link class="link" :to="{ name: 'Home' }">Home </router-link>
        </li>
        <li>
          <router-link class="link" :to="{ name: 'About' }"
            >What is LiGround?</router-link
          >
        </li>
        <li>
          <router-link class="link" :to="{ name: 'LegalInfo' }">
            Legal Info</router-link>
        </li>
        <li>
          <a class="link" href="https://github.com/ml-research/liground"
            >Go to GitHub</a
          >
        </li>

      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "navbar",
  data() {
    return {
      scrollPos: null,
    };
  },
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap");
header {
  background-color: rgba(0, 0, 0, 0.7);
  z-index: 99;
  width: 100%;
  position: fixed;
  transition: 0.5s ease all;
  color: black;

  nav {
    display: flex;
    flex-direction: row;
    padding: 12px 0;
    transition: 0.5s ease all;
    width: 90%;
    margin: 0 auto;
    @media (min-width: 1140px) {
      max-width: 1140px;
    }

    ul,
    .link {
      font-weight: 500;
      color: white;
      list-style: none;
      text-decoration: none;
      font-family: "Roboto", sans-serif;
    }

    li {
      padding: 16px;
      margin-left: 16px;
    }

    .link {
      font-size: 14px;
      transition: 0.5s ease all;
      padding-bottom: 4px;
      border-bottom: 1px solid transparent;
      font-family: "Roboto", sans-serif;
      &:hover {
        color: #00afea;
        border-color: #00afea;
      }
    }

    .branding {
      display: flex;
      align-items: center;
      img {
        width: 50px;
        transition: 0.5s ease all;
      }
    }
    .navigation {
      display: flex;
      align-items: center;
      flex: 1;
      justify-content: flex-end;
    }
  }
}
</style>
