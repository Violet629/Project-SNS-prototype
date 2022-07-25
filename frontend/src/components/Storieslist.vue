<template>
  <div class="stories-list">
    <div class="stories-list-text">
      <ul>
        <li>Stories</li>
      </ul>
      <ul>
        <li>Watch All</li>
      </ul>
    </div>
    <div class="stories-list-icon">
      <ul class="stories-list-me">
        <li>
          <img
            class="me-img"
            src="https://placeimg.com/100/100/arch"
            alt="me-img"
          />
          <p>Your Story</p>
        </li>
      </ul>
      <ul class="stories-list-friend" v-for="friendData in 3" :key="friendData">
        <li>
          <img
            class="friend-img"
            src="https://placeimg.com/100/100/arch"
            alt="friend-img"
          />
          <p>friend</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "storieslist",
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");
/* Roboto font : font-family: "Roboto", sans-serif; */

.stories-list {
  background-color: white;
  border-bottom: solid 1px #eee;
}
.stories-list-text,
.stories-list-icon {
  display: flex;
}
.stories-list-text {
  justify-content: space-between;
}
.stories-list-text ul,
.stories-list-icon ul {
  list-style: none;
  padding: 0;
}
.stories-list-text ul {
  padding-top: 0px;
  margin: 8px 16px 0px 16px;
  font-size: 14px;
  font-family: "Roboto", sans-serif;
  font-weight: 700;
}
.stories-list-me,
.stories-list-friend {
  margin: 10px;
}
.stories-list-me p,
.stories-list-friend p {
  margin: 3px 0px 0px 0px;
  text-align: center;
  font-size: 12px;
  font-family: "Roboto", sans-serif;
  font-weight: 400;
}
.me-img,
.friend-img {
  border: 2px solid transparent;
  border-radius: 50%;
  background-image: linear-gradient(#fff, #fff),
    linear-gradient(to bottom, violet 0%, orange 100%);
  background-origin: border-box;
  background-clip: content-box, border-box;
  width: 60px;
  height: 60px;
}
</style>
