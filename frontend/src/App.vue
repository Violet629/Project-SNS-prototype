<template>
  <div>
    <!-- top menu -->
    <div class="header">
      <ul>
        <li><img class="back-button" src="./assets/left.png" alt="Back" /></li>
      </ul>
      <ul>
        <li><div class="logo">Outstargram</div></li>
      </ul>
      <ul>
        <li><img class="next-button" src="./assets/right.png" alt="Next" /></li>
      </ul>
    </div>

    <!-- Storieslist -->
    <Storieslist />

    <!-- post list -->
    <Container />

    <!-- bottom menu -->
    <div class="footer">
      <ul>
        <li><img src="./assets/home2.png" alt="Home" /></li>
      </ul>
      <ul>
        <li><img src="./assets/search.png" alt="Search" /></li>
      </ul>
      <ul>
        <li><img src="./assets/add.png" alt="Add" /></li>
      </ul>
      <ul>
        <li><img src="./assets/heart.png" alt="Follow" /></li>
      </ul>
      <ul>
        <li><img src="./assets/friend.png" alt="Friend" /></li>
      </ul>
    </div>
  </div>
</template>

<script>
import Container from "./components/Container.vue";
import Storieslist from "./components/Storieslist.vue";

export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    Container,
    Storieslist,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap");
/* logo font : font-family: 'Dancing Script', cursive;*/

body {
  margin: 0;
  background: linear-gradient(
    45deg,
    #405de6,
    #5851db,
    #833ab4,
    #c13584,
    #e1306c,
    #fd1d1d
  );
}
#app {
  box-sizing: border-box;
  margin-top: 60px;
  width: 100%;
  max-width: 460px;
  margin: auto;
  border-right: 1px solid #eee;
  border-left: 1px solid #eee;
  background-color: #eee;
}
.header {
  width: 100%;
  top: 0;
  position: sticky;
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
  border-bottom: solid 1px #eee;
}
.header ul,
.footer ul {
  padding: 5px;
}
.header li,
.footer li {
  list-style: none;
}
.header img,
.footer img {
  width: 25px;
}
.logo {
  font-family: "Dancing Script", cursive;
  font-size: 25px;
}
.footer {
  width: 100%;
  position: sticky;
  display: flex;
  justify-content: space-around;
  bottom: 0;
  background-color: white;
  border-top: solid 1px #eee;
}
</style>
