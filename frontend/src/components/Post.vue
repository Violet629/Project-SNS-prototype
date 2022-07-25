<template>
  <div class="post">
    <div class="profile">
      <div class="profile-img"></div>
      <p class="profile-name">nintei</p>
    </div>
    <div class="post-img"></div>
    <div class="post-content">
      <img
        class="post-content-hearticon"
        src="../assets/heart.png"
        alt="Like"
      />
      <img
        class="post-content-commenticon"
        src="../assets/comment.png"
        alt="Comment"
      />
      <img
        class="post-content-bookmarkicon"
        src="../assets/bookmark.png"
        alt="Bookmark"
      />
      <p class="post-content-like">likes</p>
      <p class="post-content-comment">jitaisitai</p>
      <p class="post-content-tag">#</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");
/* Roboto font : font-family: "Roboto", sans-serif; */

.post {
  border-bottom: 1px solid #eee;
}
.profile {
  display: flex;
  align-items: center;
}
.profile-img {
  background-image: url("https://placeimg.com/100/100/arch");
  background-size: 100%;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  margin: 10px;
}
.profile-name {
  font-weight: bold;
  font-size: 15px;
  font-family: "Roboto", sans-serif;
  font-weight: 700;
}
.post-img {
  background-image: url("https://placeimg.com/640/480/animals");
  background-position: center;
  background-size: cover;
  height: 450px;
}
.post-content {
  margin-top: 4px;
  margin-left: 18px;
}
.post-content-hearticon,
.post-content-commenticon,
.post-content-bookmarkicon {
  width: 25px;
  margin-top: 12px;
}
.post-content-bookmarkicon {
  float: right;
  margin-right: 25px;
}
.post-content-commenticon {
  margin-left: 20px;
}
.post-content-like,
.post-content-tag {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
}
.post-content-comment {
  font-family: "Roboto", sans-serif;
}
</style>
