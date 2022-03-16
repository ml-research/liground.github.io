<template>
  <div class="about">
    <div class="bb">
      <h1>What is LiGround?</h1>
      <p>
        LiGround is a free and open-source Chess Variant Analysis GUI, which
        works with an embedded engine to allow everybody to improve their chess
        skills and efficiently analyze the most complex chess positions that
        exist. <br />
        LiGround allows its users to manually add an arbitrary engine or remove
        a specific engine if desired. This allows LiGround users to anaylize
        chess positions with an engine they prefer. <br />
        In addtition to the possibility of manually adding engines to the GUI,
        LiGround also supports a wide variaty of chess variants: Horde, King of
        the hill, racing Kings... just to name a few. To evaluate the position
        in these variants, LiGround uses Fairy Stockfish 13 as default. <br />
        The asian-chess variants Shogi, Janggi and Xiangqi are also playable
        with LiGround, as well as the evaluation of their positions.
      </p>
      <h1>A Few Impressions</h1>
      <section>
        <p>
          The standard landing page of LiGround. This is what you see when you
          open LiGround for the first time. You can deactivate the engine by
          clicking the switch button next to the name of the engine you are
          currently using. In This example Stockfish 12.
        </p>
        <img src="../assets/ligroundstart.jpeg" alt="" />
      </section>
      <section>
        <p>The asian-chess variant shogi:</p>
        <img src="../assets/shogi.jpeg" alt="" />
        <img src="../assets/shogiengine.jpeg" alt="" />
      </section>
      <section>
        <p>
          If you wish to, you can change the design of LiGround to darkmode.
          Here you can see the variant Janggi
        </p>
        <img src="../assets/janggidark.jpeg" alt="" />
      </section>
      <section>
        <p>Horde</p>
        <img src="../assets/hordedark.jpeg" alt="" />
      </section>
      <h1>
        And much more... Check it out yourself:
        <a href="https://github.com/ml-research/liground">Go To GitHub</a>
      </h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap");
.about {
  display: flex;
  align-items: center;
  justify-content: center;
  line-height: 2;
}
.bb {
  margin-top: 100px;
  margin-left: 40px;
  margin-right: 40px;
}
p {
  font-size: 20px;
  text-align: center;
  font-family: "Roboto", sans-serif;
  padding: 3em;
  padding-top: 20px;
  padding-bottom: 10px;
  margin-top: 1em;
}
h1 {
  padding: 40px;
  text-align: center;
  font-family: "Roboto", sans-serif;
}
img {
  max-height: 60%;
  max-width: 60%;
  margin-left: 300px;
  margin-top: 100px;
  margin-bottom: 50px;
  box-shadow: inset 0 0 1em black, 0 0 1em black;
}
</style>
