<template>
<div class="admin-page">
  <div class="ui grid">
    <div class="four wide column">
      <div class="ui container side-menu">
        <div class="ui vertical menu">
          <a class="active teal item">
            Create Post
          </a>
          <a class="item">
            Existing Posts
            <div class="ui label">51</div>
          </a>
        </div>
      </div>
    </div>
    <div class="twelve wide column">
      <PostList />
    </div>
  </div>
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
.container.side-menu {
  padding: 20% 5%;
}
</style>
