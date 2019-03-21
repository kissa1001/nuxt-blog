<template>
<div class="posts-page ui container">
  <h1>Featured Posts</h1>
  <div class="ui link cards">
    <PostPreview id="1" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my first post!" />
    <PostPreview id="2" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my second post!" />
    <PostPreview id="3" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my third post!" />
    <PostPreview id="4" thumbnail="https://i2-prod.chroniclelive.co.uk/incoming/article13428918.ece/ALTERNATES/s615/Crocuses-in-the-sun.jpg" title="Hello There" previewText="This is my fourth post!" />
  </div>
</div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  }
}
</script>

<style scoped>
.container {
  padding: 5%;
}
</style>
