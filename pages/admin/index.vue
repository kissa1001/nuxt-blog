<template>
<div class="admin-page">
  <div class="ui grid">
    <div class="four wide column">
      <div class="ui container side-menu">
        <div class="ui vertical menu">
          <button @click="$router.push('/admin/new-post')" class="ui primary button">
            Create Post
          </button>
          <a class="item">
            Existing Posts
            <div class="ui label">51</div>
          </a>
        </div>
      </div>
    </div>
    <div class="twelve wide column">
      <PostList isAdmin />
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
