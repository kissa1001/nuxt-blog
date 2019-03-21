<template>
<div class="home-wrapper">
  <div class="ui vertical masthead center aligned segment">
    <div class="ui text container">
      <h1 class="ui header">Get the latest tech news!</h1>
      <div class="ui animated primary button" tabindex="0">
        <div class="visible content">Check All Posts</div>
        <div class="hidden content">
          <i class="right arrow icon"></i>
        </div>
      </div>
    </div>
  </div>
  <PostList />
</div>
</template>

<script>
import PostList from '@/components/Posts/PostList'
export default {
  components: {
    PostList
  }
}
</script>

<style scoped>
.masthead.segment {
  background-color: rgb(254, 240, 60);
  min-height: 250px;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.cards {
  background-image: url('~assets/images/what-the-hex.png');
  display: flex;
  justify-content: center;
  padding-top: 5%;
}
</style>
