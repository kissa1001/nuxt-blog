<template>
<div class="posts-page ui container">
  <h1>Featured Posts</h1>
  <div class="ui link cards">
    <PostPreview id="1" :is-admin="isAdmin" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my first post!" />
    <PostPreview id="2" :is-admin="isAdmin" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my second post!" />
    <PostPreview id="3" :is-admin="isAdmin" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my third post!" />
    <PostPreview id="4" :is-admin="isAdmin" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my fourth post!" />
  </div>
</div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.container {
  padding: 5%;
}
</style>
