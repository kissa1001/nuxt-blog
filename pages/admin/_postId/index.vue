<template>
<div class="ui container">
  <h1>Edit Post</h1>
  <AdminPostForm :post="loadedPost" />
</div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'
export default {
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: 'Lina',
        title: 'My Post',
        content: 'This is a test',
        thumbnailLink: 'https://cdn.pixabay.com/photo/2018/02/09/21/46/rose-3142529__340.jpg'
      }
    }
  }
}
</script>

<style scoped>
h1 {
  margin-top: 5%;
  text-align: center;
}
</style>
