<template>
<div class="posts-page ui container">
  <h1>Featured Posts</h1>
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
