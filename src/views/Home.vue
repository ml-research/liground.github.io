<template>
  <div class="home">
    <div class="text">
      <h4>open-source, modern Chess Variant Analysis GUI</h4>
      <hr />
      <h2>LiGround</h2>
      <hr />
    </div>
    <div>
      <img src="../assets/ligroundstart.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap");
img {
  max-height: 60%;
  max-width: 60%;
  margin-left: 300px;
  margin-top: 200px;
  margin-bottom: 200px;
  box-shadow: inset 0 0 1em black, 0 0 1em black;
}
.home {
  display: flex;
  align-items: center;
  justify-content: center;
}
.text {
  padding-left: 100px;

  h4 {
    text-transform: uppercase;
    font-size: 15px;
    padding-bottom: 4px;
    font-family: "Roboto", sans-serif;
  }
  h2 {
    font-size: 50px;
    font-family: "Roboto", sans-serif;
    @media (min-width: 550px) {
      font-size: 80px;
    }
  }
  hr:nth-child(2) {
    max-width: 365px;
    margin-bottom: 16px;
    font-family: "Roboto", sans-serif;
  }
  hr:nth-child(4) {
    height: 6px;
    background-color: black;
    border: none;
    max-width: 85px;
    margin-top: 16px;
    font-family: "Roboto", sans-serif;
  }
}
</style>
