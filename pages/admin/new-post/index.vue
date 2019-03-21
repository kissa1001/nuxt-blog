<template>
<div class="ui container">
  <h1>Create Post</h1>
  <AdminPostForm />
</div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'
export default {
  components: {
    AdminPostForm
  }
}
</script>

<style scoped>
h1 {
  margin-top: 5%;
  text-align: center;
}
</style>
